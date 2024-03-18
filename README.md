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
-  2 Tables: 
  - 1 new table (Intake, new_intake)
  - Changes to the Contact table 
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
