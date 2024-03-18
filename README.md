# DataverseGranularSearch
Contains Managed and Unmanaged exports of the Granular Search solution delivered in the Microsoft Federal Business Applications Customer Success Power Hour 2024-03-18

# Summary:
- 11 components total; 
-  5 Script Web Resources
-  2 Tables
-  2 Apps
-  1 Site map
-  1 Security Role

# Detail:
-  5 Script Web Resources
   - new_intake_nofacade.js (standalone, self contained script used on the Intake form named 'No Facade (better)'. This is a script written directly against Dataverse client scripting API methods.)
   - sdk.js (script 1of4 used on the Intake form named 'Intake (best)'. This is the root namespace (SDK) script containing constants and project-specific enumerations)
   - globalfunctions.js (script 2of4 used on the Intake form named 'Intake (best)'. This is the (SDK.global) namespace script containing generic functions to be used in any project)
   - new_intake.js (script 3of4 used on the Intake form named 'Intake (best)'. This is the (SDK.new_intake) namespace script that is specific to the Intake entity form)
   - new_granularsearch.js (script 4of4 used on the Intake form named 'Intake (best)'. This is the (SDK.new_granularsearch) namespace script that compartmentalizes the Granular search implementation into a separate file)
-  2 Tables: 
  - Intake, (new_intake) - new
  - Contact, (contact) - out of the box table with a few changes
    - 4 text fields added
    - layout and Find Column changes to Quick Find Active Contacts view and Contacts Lookup View
    - One 1:N relationship between Contact and Intake
-  2 Apps: 
  - Granular Search (Model Driven, includes 1 site map) 
  - Granular Search - Canvas (Canvas)
-  1 Security Role: a copy of Basic User named "Basic User - Copy" which adds privileges to the Intake table to the least privileged security role that ships with Dataverse.

# Recommendations
It is strongly recommended that the Unmanaged copy of the solution be used:
- In a non-production instance of Dataverse
- In a dataverse instance where the changes described above are acceptable
- In an environment instance where changes to the app(s) are to be made.

Otherwise, use the Managed copy of the solution. 
It will allow:
- the changes to be contained in a Managed layer, thus allowing you the opportunity to import, Run, and then Delete the solution when finished.
It will not allow:
- changes to be made to the imported solution or applications.
