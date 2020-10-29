
In Oracle R12 Database, oracle introduced the database object versioning concepts 

For new table creations use
```sql
execute AD_ZD_TABLE.UPGRADE('XXCUST','XX_CUST_TBL1');
```

For exisitng table alterations use
```sql
execute AD_ZD_TABLE.PATCH('XXCUST','XX_CUST_TBL1')
```

For table grants use
```sql
execute AD_ZD.GRANT_PRIVS('SELECT','XX_CUST_TBL1','XX_ROLE0')
```