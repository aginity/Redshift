The table below details all queries within the Aginity-Pro-Redshift-Admin-Set1 package.



|Catalog Item Name               |Catalog Item Package            |Catalog Item Description            | Required Table     |
|--------------------------      |--------------------------------|------------------------------------|--------------------|
|Active queries|Aginity-Pro-Redshift-Admin-Set1.aginitypkg| This query allows you to see active queries running on the Redshift database|stv_inflight|
|Active sessions|Aginity-Pro-Redshift-Admin-Set1.aginitypkg| This query allows you to see active sessions running on the Redshift database|stv_sessions, stv_recents|
|Column compression by partial table name|Aginity-Pro-Redshift-Admin-Set1.aginitypkg| This query allows you to see a list of columns within a table and their corresponding compression type|pg_table_def|
|Deadlocks|Aginity-Pro-Redshift-Admin-Set1.aginitypkg| This query allows you to see deadlocks on competing queries|stv_locks|
|Get Constraints for an Object|Aginity-Pro-Redshift-Admin-Set1.aginitypkg| This query allows you to see defined database constraints|pg_class, pg_namespace,relnamespace,pg_contraint,pg_class|
