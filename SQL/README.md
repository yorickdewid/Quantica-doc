
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

Function can be called directly from the SQL interface using the `select` operation. For example

```sql
SELECT MD5("w00t!);
```


## Insert

Data can be inserted into the database as separate entities or as part of an existing object. To insert a single value

```sql
INSERT VALUES("BSD");
```
Or

```sql
INSERT INTO NULL VALUES("BSD-3");
```

Or an array of values

```sql
INSERT VALUES("BSD", "MIT", "GPL", "Apache");
```

To create an object also the definition must be given. The definition can be seen as keys in an object.

```sql
INSERT INTO NULL ("name", "year", "unix") VALUES ("Linux", 1991, true);
```
