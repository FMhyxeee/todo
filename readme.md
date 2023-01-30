# TODO

todo can create a new todo list, add items to the list, mark items as done, and remove items from the list.

todo has will have backends with sqlite. and frontends with tauri.

## Backends
use sqlx and sqlite
we have a 
```rust
pub struct Todo {
    id: i32,
    created: DateTime<Utc>,
    title: String,
    done: bool,
}
```

```sql
CREATE TABLE TODO (
    id INTEGER PRIMARY KEY,
    created DATETIME,
    title TEXT,
    done BOOLEAN
)
```