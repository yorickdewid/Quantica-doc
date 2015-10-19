
# SQL interface

The SQL interface allows for direct queries on the database much like traditional RDBMS do. It does not conform to any SQL standard, but most queries can be written similar.

## Select


Select data from a key.

```sql
SELECT <fields> FROM '<QUID>';
```

For example

```sql
SELECT * FROM '00000000-0000-0000-0000-000000000000';
```

Keys can also be written in the full QUID notation as `"{00000000-00c1-a150-0000-000000000080}"` encapsulated in double quotes.