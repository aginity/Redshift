# Redshift Administrative Queries for Aginity Pro or Team

This repository has useful Redshift data dictionary/DBA queries you can use to do common database related tasks. You can take any of the aginitypkg files and immediately import them into Aginity Pro and Team.


To get started with this sample a few pre-requisites:

1. You must have access to a Redshift database
2. The queries here will reference the following data dictionary tables.
    * INFORMATION_SCHEMA.TABLES
    * INFORMATION_SCHEMA.COLUMNS
    
# How to Import Queries Packages into Aginity Pro or Team

1. To import download one of all of the <name>.aginitypkg files in the Github repository
2. Open Aginity Pro or Team and use the File Import method as shown below

![File Import Image!](/images/importPkg.png "Import Aginity Catalog Package")

3. You will be presented with an Import Wizard as shown below.

![File Import Wizard!](/images/importWiz.png "Import Aginity Catalog Package Wizard")

4. Pick a destination directory you want to place the catalog queries into.  I recommend for Redshift Utility queries specifyng a head directory like "Redshift Utility Queries"
5. Typically you can click All or select the scripts you want to import
6. Voila!  You are ready to use the queries.

# Using Imported Queries

