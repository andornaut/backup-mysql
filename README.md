# backup-remote-mysql

Backup from and restore to remote MySQL or MariaDB databases.

## Backup with [backupmysql](./backupmysql)

### Example

```
$ ./backupmysql user@example.com backup.gz
```

### Usage

```
backupmysql host [backup_file]
```

Argument | Required |Description
--- | --- | ---
host | ✓ | The remote host to connect to
backup_file | | The optional file to which to save the backup data. If not specified, then the backup data will be written to stdout

## Restore with [restoremysql](./restoremysql)

### Example

```
$ ./restoremysql user@example.com backup.gz
```

### Usage

```
./restoremysql host [backup_file]
```

Argument | Required |Description
--- | --- | ---
host | ✓ | The remote host to connect to
backup_file | | The optional file from which to read the backup data. If not specified, then the backup data will be read from stdin

