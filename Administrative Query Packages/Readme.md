# Redshift Package Summary

|Package Name| Package Description| Number of Queries in Package|
|------------|--------------------|-----------------------------|
|Aginity-Pro-Redshift-Admin-Set1|Contains administrative queries to do common tasks in Redshift   | 8  |
|Aginity-Pro-Redshift-Table-Column-Search   | Contains search queries to find where tables or columns exist within Redshift   | 6  |
|Aginity-Pro-Redshift-Table-Distribution-Skew-Info   | Contains queries to show skew and distribution for tables in Redshift   | 2  |
|Aginity-Pro-Redshift-User-Permissions   | Contains queries to show permissions on objects   | 3  |


### The table below details all queries within the Aginity-Pro-Redshift-Admin-Set1 package.



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


### The table below details all queries within the Aginity-Pro-Redshift-Table-Column-Search-Queries package.



|Catalog Item Name               |Catalog Item Description            | Required Table     |
|--------------------------      |------------------------------------|--------------------|
|Search for Columns by exact name - All schemas       | This query allows you to search for any column across all schemas with an exact name match|INFORMATION_SCHEMA.COLUMNS|
|Search for Columns by exact name - Public schema|This query allows you to search for any column across Public schema with an exact name match|INFORMATION_SCHEMA.COLUMNS|
|Search for Columns by partial name - All schema|This query allows you to search for any column across all schemas with a partial name match|INFORMATION_SCHEMA.COLUMNS|
|Search for Columns by partial name - Public schema|This query allows you to search for any column across Public schemas with a partial name match|INFORMATION_SCHEMA.COLUMNS|
|Search for Tables by partial name - All schema|This query allows you to search for any table across all schemas with a partial name match|INFORMATION_SCHEMA.COLUMNS|
|Search for Tables by partial name - Public schema|This query allows you to search for any table across Public schemas with a partial name match|INFORMATION_SCHEMA.COLUMNS|

### The table below details all queries within the Aginity-Pro-Redshift-Table-Distribution-Skew-Info package.

|Catalog Item Name               |Catalog Item Description            | Required Table     |
|--------------------------      |------------------------------------|--------------------|
|Distribution and skew for all tables in database | This query shows information about distribution and skew for all tables in database|svv_table_info, stv_blocklist|
|Distribution and skew the table  |This query shows information about distribution and skew for the particular table|svv_table_info, stv_blocklist|


### The table below details all queries within the Aginity-Pro-Redshift-User-Permissions package.

|Catalog Item Name               |Catalog Item Description            | Required Table     |
|--------------------------      |------------------------------------|--------------------|
|User permissions on tables in database for particular user | This query shows information about user's permissions on tables|pg_tables, pg_user|
|Users' permissions on table | This query shows information on permissions for particular table|pg_tables, pg_user|
|Users permissions on all objects in database | This query shows all permissions on all objects for all users in database|pg_tables, pg_user, pg_group, pg_language, pg_default_acl, pg_proc, pg_database, pg_class, pg_namespace|

