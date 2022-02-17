# Initializing Database (POSTGRESQL)
- Create new user
- Create new database
- Set user as owner of database
- Run the following commands for single user access:
```
REVOKE connect ON DATABASE "databaseName" FROM PUBLIC;
GRANT connect ON DATABASE "databaseName" TO "role/user";
```
- NOTE: Superusers can still connect