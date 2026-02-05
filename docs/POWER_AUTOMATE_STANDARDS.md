\# Power Automate Standards (Dyn→SN)



\## Naming

\- \*\*Flow\*\*: `DYNtoSN\_<Process>\_<Trigger>`

\- \*\*Actions\*\*: `Verb\_Object\[\_Qualifier]`

\- \*\*Variables\*\*: `var<System><Meaning>`

\- \*\*Scopes\*\*: `SCP\_Try`, `SCP\_Catch`, `SCP\_Finally`

\- \*\*Connection references\*\*: `CR\_<System>\_<Purpose>`

\- \*\*Child flows\*\*: `CF\_<Process>\_<Action>`



\## Field \& table references

\- Use logical names from the Data Dictionary (e.g., `exp\_Name`).

\- Read rows safely with null‑safe navigation and defaults.



\*\*Examples\*\*

\- First row: `@{first(body('List\_<Entity>')?\['value'])}`

\- Read field: `@{first(body('List\_Project\_Template')?\['value'])?\['exp\_name']}`

\- Default: `@{coalesce(first(body('List\_Project\_Template')?\['value'])?\['exp\_projecttemplate'], 'Unknown')}`

\- One match check:  

&nbsp; `@{if(equals(length(body('List\_Project\_Template')?\['value']), 1), 'OK', 'AMBIG\_OR\_MISSING')}`

\- Correlation key:  

&nbsp; `@{concat(variables('varDYNCompanyID'), '|', variables('varSNID'))}`



\## Data validation

\- \*\*Null/presence\*\*: `coalesce`, `empty`, `length` checks.

\- \*\*Type\*\*: `int()` / `float()` before maths.

\- \*\*Dates\*\*: ISO‑8601 via `formatDateTime()`.

\- \*\*GUIDs\*\*: length/dash checks, as required by target system.

\- \*\*Choices/labels\*\*: verify membership before branching.

\- \*\*Lookups\*\*: confirm related row exists before writing FK.

\- \*\*List size\*\*: `0 = Not found`; `>1 = Ambiguous`.



\## Idempotency

\- Design a correlation key.  

\- Check for existing record before Create; prefer Upsert if available.



\## Error handling

\- \*\*Scopes\*\*: `SCP\_Try → SCP\_Catch → SCP\_Finally`.

\- \*\*Catch\*\*: build an error object (`flow`, `correlationId`, `lastAction`, `code`, `message`, `utcTime`).

\- \*\*Terminate\*\*: Validation = `BadRequest`; Transient = retry/backoff.

\- \*\*Log\*\*: Write to `Integration Logs` with key fields for triage.



\## Flow Dictionary usage

\- Create a Flow Dictionary for each flow.

\- Two tabs: \*\*Calculated References\*\* and \*\*Manual References\*\*.

\- Columns: `Action | Action Type | Friendly Name | Variable | Value | Example | Flow Reference`.

