\# Connector References \& Design Notes



Use these official pages when proposing connector steps, limits, auth, and throttling.



\## Connector catalog (hub)

\- Microsoft Learn: \*\*Connector reference overview\*\*  

&nbsp; https://learn.microsoft.com/en-us/connectors/connector-reference/



\## ServiceNow

\- Microsoft Learn: \*\*ServiceNow – Connectors\*\*  

&nbsp; https://learn.microsoft.com/en-us/connectors/service-now/

\- Notes:

&nbsp; - The connector is available across most Power Automate regions; it supports CRUD for common tables.  

&nbsp; - Known limitations include instance URL/domain considerations and some field behaviours on Create Record.  

&nbsp; - If using Entra ID OAuth or alternative domains, follow the Learn guidance for setup and troubleshooting.



\## Project Online

\- Microsoft Learn: \*\*Project Online – Connectors\*\*  

&nbsp; https://learn.microsoft.com/en-us/connectors/projectonline/

\- Notes:

&nbsp; - Requires a valid \*\*PWA root site URL\*\* (SharePoint Online) to connect.  

&nbsp; - Throttling: typical limit of \*\*100 calls per 60 seconds per connection\*\*.  

&nbsp; - Common actions: create project, create task, list projects/tasks.



\## Microsoft Teams

\- Microsoft Learn: \*\*Microsoft Teams – Connectors\*\*  

&nbsp; https://learn.microsoft.com/en-us/connectors/teams/

\- Notes:

&nbsp; - Posting actions have a \*\*~28 KB message size\*\* limit (includes HTML and mentions).  

&nbsp; - Some actions require the \*\*Workflows (Power Automate) app\*\* allowed in Teams admin.



\## Microsoft Dataverse

\- Microsoft Learn: \*\*Microsoft Dataverse – Connectors\*\*  

&nbsp; https://learn.microsoft.com/en-us/connectors/commondataserviceforapps/

\- Notes:

&nbsp; - Premium connector.  

&nbsp; - Supports multiple auth types (including \*\*Service Principal\*\* and \*\*Certificate\*\*).  

&nbsp; - Use logical names; handle paging/filtering for list operations.



\## Office 365 Outlook

\- Microsoft Learn: \*\*Office 365 Outlook – Connectors\*\*  

&nbsp; https://learn.microsoft.com/en-us/connectors/office365/

\- Notes:

&nbsp; - Watch for \*\*deprecated operations\*\* and client constraints for \*\*actionable messages\*\*.  

&nbsp; - Some operations surface Microsoft Graph behaviours and limitations.



> Always cite the Learn page when claiming a limit or behaviour in a design.

