\# Dyn→SN Integration Knowledge Base



This repository hosts the public documentation used by the \*\*Dyn→SN Integration Assistant\*\* (a Custom Copilot in M365).  

It contains the standards, data dictionary, connector notes, and the agent system prompt.



\## Files

\- `docs/AGENT\_PROMPT.md` – System instructions for the Custom Copilot (paste into the Instructions box).

\- `docs/POWER\_AUTOMATE\_STANDARDS.md` – Naming, validation, and error-handling standards.

\- `docs/FLOW\_DICTIONARY\_TEMPLATE.md` – How to fill the Flow Dictionary for each flow.

\- `docs/DATA\_DICTIONARY.md` – Tables and columns used in this integration (from project sources).

\- `docs/CONNECTOR\_REFERENCES.md` – Connector links + design notes.



\## How to use with M365 Custom Copilot

1\. Create a \*\*Custom Copilot\*\* (Start from scratch).  

2\. Open `docs/AGENT\_PROMPT.md` and paste its content into \*\*Instructions\*\*.  

3\. Add each file’s \*\*RAW\*\* GitHub URL as a \*\*Website\*\* knowledge source.  

4\. Also add Microsoft Learn pages for the connectors (see `docs/CONNECTOR\_REFERENCES.md`).  

5\. Save and test.



> M365 Custom Copilot does not support direct file uploads. Use public URLs (GitHub raw links) or SharePoint pages.

