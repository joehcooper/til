# Find Drupal Database Type And Version

## CLI

```
./drush sql-query "SELECT VERSION();"

# You can also use the shorthand 'sqlq' alias:
./drush sqlq "SELECT VERSION();"
```

Example Outputs:
- MySQL: 9.7
- MariaDB: 12.3-MariaDB

While running `./drush status` will tell you the database driver _(e.g., mysql)_, querying the database directly using `sql-query` is the most reliable way to get the exact type and version number your environment is currently running.
