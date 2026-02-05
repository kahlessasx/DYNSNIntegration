\# Data Dictionary (Dyn→SN)



Below are the key custom tables and fields used by the integration.  

\*\*PK\*\* = Unique identifier; \*\*FK\*\* = Lookup.



---



\## Company Mapping

| Display Name     | Logical Name           | Data Type               | PK | FK | Notes                 |

|------------------|------------------------|-------------------------|----|----|----------------------|

| Company Code     | exp\_CompanyCode        | Single line of text     |    |    |                      |

| Company GUID     | exp\_CompanyGUID        | Single line of text     |    |    |                      |

| Company Mapping  | exp\_CompanyMappingId   | Unique identifier       | ✔  |    | Primary key          |

| Company Name     | exp\_Name               | Single line of text     |    |    | Primary name column  |

| Company Sys\_ID   | exp\_CompanySys\_ID      | Single line of text     |    |    |                      |

| Dynamics Name    | exp\_DynamicsName       | Single line of text     |    |    |                      |

| Teams Channel    | exp\_TeamsChannel       | Single line of text     |    |    |                      |



---



\## GTM Area Mapping

| Display Name         | Logical Name            | Data Type               | PK | FK | Notes                |

|----------------------|-------------------------|-------------------------|----|----|---------------------|

| Azure AD Object ID   | exp\_AzureADObjectID     | Single line of text     |    |    |                     |

| BFS                  | exp\_BFS                 | Yes/No                  |    |    |                     |

| C\&G                  | exp\_CG                  | Yes/No                  |    |    |                     |

| DYN Title            | exp\_DYNTitle            | Single line of text     |    |    |                     |

| Dynamics GUID        | exp\_DynamicsGUID        | Single line of text     |    |    |                     |

| email                | exp\_email               | Single line of text     |    |    |                     |

| Full Name            | exp\_Name                | Single line of text     |    |    | Primary name column |

| GTM Area Mapping     | exp\_GTMAreaMappingId    | Unique identifier       | ✔  |    | Primary key         |

| SN ID                | exp\_SNID                | Single line of text     |    |    |                     |

| SN Title             | exp\_SNTitle             | Single line of text     |    |    |                     |



---



\## Opportunity Mapping

| Display Name          | Logical Name              | Data Type               | PK | FK | Notes                |

|-----------------------|---------------------------|-------------------------|----|----|---------------------|

| DynOpportunity GUID   | exp\_DynOpportunityGUID    | Single line of text     |    |    |                     |

| Opportunity Mapping   | exp\_OpportunityMappingId  | Unique identifier       | ✔  |    | Primary key         |

| Primary Column        | exp\_PrimaryColumn         | Single line of text     |    |    |                     |

| Project Name          | exp\_Name                  | Single line of text     |    |    | Primary name column |

| SN Sys\_id             | exp\_SNSys\_id              | Single line of text     |    |    |                     |



---



\## Template Mapping

| Display Name              | Logical Name                | Data Type               | PK | FK | Notes                |

|---------------------------|-----------------------------|-------------------------|----|----|---------------------|

| DynamicsGUID              | exp\_DynamicsGUID            | Single line of text     |    |    |                     |

| Effort                    | exp\_Effort                  | Whole number            |    |    |                     |

| Opportunity Type          | exp\_Name                    | Single line of text     |    |    | Primary name column |

| Project Template          | exp\_ProjectTemplate         | Single line of text     |    |    |                     |

| Project Template SysID    | exp\_ProjectTemplateSysID    | Single line of text     |    |    |                     |

| Template Mapping          | exp\_TemplateMappingId       | Unique identifier       | ✔  |    | Primary key         |

| uomid                     | exp\_uomid                   | Single line of text     |    |    |                     |



---



\## User Mapping

| Display Name        | Logical Name          | Data Type               | PK | FK | Notes                |

|---------------------|-----------------------|-------------------------|----|----|---------------------|

| DYN Name            | exp\_DYNName           | Single line of text     |    |    |                     |

| DYN Resource GUID   | exp\_DYNGUID           | Single line of text     |    |    |                     |

| DYN UPN             | exp\_DYNUPN            | Single line of text     |    |    |                     |

| DYN User GUID       | exp\_DYNUserGUID       | Single line of text     |    |    |                     |

| Email               | exp\_DYNEmail          | Single line of text     |    |    |                     |

| Full Name           | exp\_Name              | Single line of text     |    |    | Primary name column |

| SN ID               | exp\_SNID              | Single line of text     |    |    |                     |

| SN Name             | exp\_SNName            | Single line of text     |    |    |                     |

| SN Title            | exp\_SNTitle           | Single line of text     |    |    |                     |

| SN ZZZ Username     | exp\_ZZZUsername       | Single line of text     |    |    |                     |

| User Mapping        | exp\_UserMappingId     | Unique identifier       | ✔  |    | Primary key         |



---



\## Project Mapping

| Display Name        | Logical Name          | Data Type               | PK | FK | Notes                |

|---------------------|-----------------------|-------------------------|----|----|---------------------|

| DYN Lead            | exp\_DYNLead           | Single line of text     |    |    |                     |

| DYN Lead SN ID      | exp\_DYNLeadSNID       | Single line of text     |    |    |                     |

| DYN Project GUID    | exp\_DYNProjectGUID    | Single line of text     |    |    |                     |

| DYN QUO             | exp\_DYNQUO            | Single line of text     |    |    |                     |

| Project Mapping     | exp\_ProjectMappingId  | Unique identifier       | ✔  |    | Primary key         |

| Project Name        | exp\_Name              | Single line of text     |    |    | Primary name column |

| SN BIL              | exp\_SNBIL             | Single line of text     |    |    |                     |

| SN Company ID       | exp\_SNCompanyID       | Single line of text     |    |    |                     |

| SN ID               | exp\_SNID              | Single line of text     |    |    |                     |

| SN PRJ              | exp\_SNPRJ             | Single line of text     |    |    |                     |

| SN Template ID      | exp\_SNTemplateID      | Single line of text     |    |    |                     |



---



\## Project Task Mapping

| Display Name                    | Logical Name                   | Data Type               | PK | FK | Notes                |

|---------------------------------|--------------------------------|-------------------------|----|----|---------------------|

| Day Rate                        | exp\_DayRate                    | Currency                |    |    |                     |

| Day Rate (Base)                 | exp\_dayrate\_Base               | Currency                |    |    |                     |

| DYN Assigned Resource           | exp\_DYNAssignedResource        | Single line of text     |    |    |                     |

| DYN Assigned Resource GUID      | exp\_DYNAssignedResourceGUID    | Single line of text     |    |    |                     |

| DYN GUID                        | exp\_DYNGUID                    | Single line of text     |    |    |                     |

| Effort                          | exp\_Effort                     | Single line of text     |    |    |                     |

| Project Task Mapping            | exp\_ProjectTaskMappingId       | Unique identifier       | ✔  |    | Primary key         |

| Project Task Name               | exp\_Name                       | Single line of text     |    |    | Primary name column |

| SN Additional Resource IDs      | exp\_SNAdditionalResourceIDs    | Single line of text     |    |    |                     |

| SN Assigned Resource            | exp\_SNAssignedResource         | Single line of text     |    |    |                     |

| SN Assigned Resource ID         | exp\_SNAssignedResourceID       | Single line of text     |    |    |                     |



---



\## Time Mapping

| Display Name        | Logical Name        | Data Type         | PK | FK | Notes                               |

|---------------------|---------------------|-------------------|----|----|--------------------------------------|

| DYN Duration        | exp\_DYNDuration     | Decimal           |    |    |                                      |

| DYN Project GUID    | exp\_DYNProjectGUID  | Lookup            |    | ✔  | Foreign key                          |

| DYN Project Task    | exp\_DYNProjectTask  | Lookup            |    | ✔  | Foreign key                          |

| DYN Resource        | exp\_DYNResource     | Lookup            |    | ✔  | Foreign key                          |

| Name                | exp\_Name            | Single line of text |  |    | Primary name column                  |

| SN Fri              | exp\_SNFri           | Decimal           |    |    |                                      |

| SN Mon              | exp\_SNMon           | Decimal           |    |    |                                      |

| SN Sat              | exp\_SNSat           | Decimal           |    |    |                                      |

| SN Sun              | exp\_SNSun           | Decimal           |    |    |                                      |

| SN Thurs            | exp\_SNThurs         | Decimal           |    |    |                                      |

| SN Time Card ID     | exp\_SNTimeCardID    | Single line of text |  |    |                                      |

| SN TimeSheet ID     | exp\_SNTimeSheetID   | Single line of text |  |    |                                      |

| SN Tues             | exp\_SNTues          | Decimal           |    |    |                                      |

| SN WC               | exp\_SNWC            | Date only         |    |    | Week commencing                      |

| SN Wed              | exp\_SNWed           | Decimal           |    |    |                                      |

| Time Mapping        | exp\_TimeMappingId   | Unique identifier | ✔  |    | Primary key                          |

