# Redshift Administrative Queries for Aginity Pro or Team

This repository has useful Redshift data dictionary/DBA queries you can use to do common database related tasks. You can take any of the aginitypkg files and immediately import them into Aginity Pro and Team.


To get started with this sample a few pre-requisites:

1. You must have access to a Redshift database and appropriate permissions to the INFORMATION_SCHEMA.
2. The table below provides a reference to the INFORMATION_SCHEMA tables used and the corresponding catalog query names and description.

|Catalog Item Name               |Catalog Item Package            |Catalog Item Description            | Required Table     |
|--------------------------      |--------------------------------|------------------------------------|--------------------|
|Search for Columns by           
 exact name - All schemas        |Aginity-Pro-Redshift-Table-Column-Search-Queries.aginitypkg| This query allows you to search for any column across all schemas with an exact name match|INFORMATION_SCHEMA.COLUMNS|
|Search for Columns by exact name - Public schema|Aginity-Pro-Redshift-Table-Column-Search-Queries.aginitypkg| This query allows you to search for any column across Public schema with an exact name match|INFORMATION_SCHEMA.COLUMNS|
    
# How to Import Queries Packages into Aginity Pro or Team

1. To import download one of all of the <name>.aginitypkg files in the Github repository
2. Open Aginity Pro or Team and use the File Import method as shown below

![File Import Image!](/images/importPkg.png "Import Aginity Catalog Package")

3. You will be presented with an Import Wizard as shown below.

![File Import Wizard!](/images/ImportWiz.png "Import Aginity Catalog Package Wizard")

4. Pick a destination directory you want to place the catalog queries into.  I recommend for Redshift Utility queries specifyng a head directory like "Redshift Utility Queries"
5. Typically you can click All or select the scripts you want to import
6. Voila!  You are ready to use the queries.

# Using Imported Queries

1. You can call a catalog item by double clicking on the name of it from within the Catalog Browser as show below

![Reference Catalog!](/images/dblClick.png "Call Catalog")

2. Hit the execute button within a query window and enter your prompt as shown below

![Parameter!](/images/pickParam.png "Enter Parameter")

3. Enjoy the results and not having to write this query ever again!

![View Results!](/images/viewResult.png "View Results")
