\# Flow Dictionary – Template \& Guide



Use one Flow Dictionary per flow.



\## Tabs

\- \*\*Calculated References\*\* – values read from triggers/actions (Dataverse, ServiceNow, Project Online, Teams, Outlook).

\- \*\*Manual References\*\* – constants and Compose outputs.



\## Columns (in this exact order)

`Action | Action Type | Friendly Name | Variable | Value | Example | Flow Reference`



\### Column guidance

\- \*\*Action\*\*: exact step name (e.g., `Get\_Project\_Template`).

\- \*\*Action Type\*\*: connector + operation (e.g., `Dataverse – List rows`).

\- \*\*Friendly Name\*\*: business label (e.g., “SN Template ID”).

\- \*\*Variable\*\*: the internal variable name (e.g., `varSNTemplateID`).

\- \*\*Value\*\*: logical field (e.g., `exp\_projecttemplatesysid`).

\- \*\*Example\*\*: a real sample value from a test run.

\- \*\*Flow Reference\*\*: paste‑ready expression, null‑safe:

&nbsp; - `@{body('Get\_Project\_Template')?\['value']?\[0]?\['exp\_projecttemplatesysid']}`



> Tip: Enforce single‑row expectations with a length check before using index `\[0]`.

