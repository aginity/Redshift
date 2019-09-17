# Redshift Package Summary

|Package Name| Package Description| Number of Queries in Package|
|------------|--------------------|-----------------------------|
|Aginity-Pro-Redshift-Admin-Set1|Contains administrative queries to do common tasks in Redshift   | 8  |
|Aginity-Pro-Redshift-Table-Column-Search   | Contains search queries to find where tables or columns exist within Redshift   | 6  |



### The table below details all queries within the [Aginity-Pro-Redshift-Admin-Set1](https://github.com/aginity/Redshift/blob/master/Administrative%20Query%20Packages/Aginity-Pro-Redshift-Admin-Set1.aginitypkg) package.



|Catalog Item Name               |Catalog Item Description            | Required Table     |
|--------------------------|------------------------------------|--------------------|
|Active queries|This query allows you to see active queries running on the Redshift database|stv_inflight|
|Active sessions|This query allows you to see active sessions running on the Redshift database|stv_sessions, stv_recents|
|Column compression by partial table name|This query allows you to see a list of columns within a table and their corresponding compression type|pg_table_def|
|Deadlocks|This query allows you to see deadlocks on competing queries|stv_locks|
|Get Constraints for an Object|This query allows you to see defined database constraints|pg_class, pg_namespace,relnamespace,pg_contraint,pg_class|
|get DDL for a View|This will produce the SQL required for compiling a view|pg_class, pg_namespace|
|get information for COPY runs for last N days|This query will show you what data has been loaded(COPY) into Redshift in the last n days|stl_s3client, stl_query|
|get View dependency|This query will list all dependent table names a view uses |pg_class, pg_depend   |


### The table below details all queries within the [Aginity-Pro-Redshift-Table-Column-Search-Queries](https://github.com/aginity/Redshift/blob/master/Administrative%20Query%20Packages/Aginity-Pro-Redshift-Table-Column-Search-Queries.aginitypkg) package.



|Catalog Item Name               |Catalog Item Description            | Required Table     |
|--------------------------      |------------------------------------|--------------------|
|Search for Columns by exact name - All schemas       | This query allows you to search for any column across all schemas with an exact name match|INFORMATION_SCHEMA.COLUMNS|
|Search for Columns by exact name - Public schema|This query allows you to search for any column across Public schema with an exact name match|INFORMATION_SCHEMA.COLUMNS|
|Search for Columns by partial name - All schema|This query allows you to search for any column across all schemas with a partial name match|INFORMATION_SCHEMA.COLUMNS|
|Search for Columns by partial name - Public schema|This query allows you to search for any column across Public schemas with a partial name match|INFORMATION_SCHEMA.COLUMNS|
|Search for Tables by partial name - All schema|This query allows you to search for any table across all schemas with a partial name match|INFORMATION_SCHEMA.COLUMNS|
|Search for Tables by partial name - Public schema|This query allows you to search for any table across Public schemas with a partial name match|INFORMATION_SCHEMA.COLUMNS|
