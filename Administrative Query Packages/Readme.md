The table below details all queries within the Aginity-Pro-Redshift-Admin-Set1 package.



|Catalog Item Name               |Catalog Item Package            |Catalog Item Description            | Required Table     |
|--------------------------      |--------------------------------|------------------------------------|--------------------|
|Active queries|Aginity-Pro-Redshift-Admin-Set1.aginitypkg| This query allows you to see active queries running on the Redshift database|stv_inflight|
|Active sessions|Aginity-Pro-Redshift-Admin-Set1.aginitypkg| This query allows you to see active sessions running on the Redshift database|stv_sessions, stv_recents|
|Column compression by partial table name|Aginity-Pro-Redshift-Admin-Set1.aginitypkg| This query allows you to see a list of columns within a table and their corresponding compression type|pg_table_def|
|Deadlocks|Aginity-Pro-Redshift-Admin-Set1.aginitypkg| This query allows you to see deadlocks on competing queries|stv_locks|
|Get Constraints for an Object|Aginity-Pro-Redshift-Admin-Set1.aginitypkg| This query allows you to see defined database constraints|pg_class, pg_namespace,relnamespace,pg_contraint,pg_class|


The table below details all queries within the Aginity-Pro-Redshift-Table-Column-Search-Queries package.



|Catalog Item Name               |Catalog Item Package            |Catalog Item Description            | Required Table     |
|--------------------------      |--------------------------------|------------------------------------|--------------------|
|Search for Columns by exact name - All schemas        |Aginity-Pro-Redshift-Table-Column-Search-Queries.aginitypkg| This query allows you to search for any column across all schemas with an exact name match|INFORMATION_SCHEMA.COLUMNS|
|Search for Columns by exact name - Public schema|Aginity-Pro-Redshift-Table-Column-Search-Queries.aginitypkg| This query allows you to search for any column across Public schema with an exact name match|INFORMATION_SCHEMA.COLUMNS|
|Search for Columns by partial name - All schema|Aginity-Pro-Redshift-Table-Column-Search-Queries.aginitypkg| This query allows you to search for any column across all schemas with a partial name match|INFORMATION_SCHEMA.COLUMNS|
|Search for Columns by partial name - Public schema|Aginity-Pro-Redshift-Table-Column-Search-Queries.aginitypkg| This query allows you to search for any column across Public schemas with a partial name match|INFORMATION_SCHEMA.COLUMNS|
|Search for Tables by partial name - All schema|Aginity-Pro-Redshift-Table-Column-Search-Queries.aginitypkg| This query allows you to search for any table across all schemas with a partial name match|INFORMATION_SCHEMA.COLUMNS|
|Search for Tables by partial name - Public schema|Aginity-Pro-Redshift-Table-Column-Search-Queries.aginitypkg| This query allows you to search for any table across Public schemas with a partial name match|INFORMATION_SCHEMA.COLUMNS|

