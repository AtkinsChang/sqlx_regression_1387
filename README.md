# SQLx Regression 1387 

`./todos` is taken and modified from [official example](https://github.com/launchbadge/sqlx/tree/ab/fix-query-file/examples/sqlite/todos)

## Reproduce Step

1. Declare the database URL

```bash
export DATABASE_URL="sqlite:${PWD}/todos.db"
```

2. Create the database.

```bash
sqlx db create
```

3. Run sql migrations

```bash
pushd todos && sqlx migrate run && popd
```

4. Build

```bash
cargo build
```
