# backup-remote-mysql

Backup from and restore to MySQL or MariaDB databases.

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
host | ✓ | The remote host to connect to. If set to "localhost", then a remote connection will not be attempted.
backup_file | | The optional file to which to save the backup data. If not specified, then the backup data will be written to stdout

## Restore with [restoremysql](./restoremysql)

### Example

```
$ ./restoremysql localhost backup.gz
```

### Usage

```
./restoremysql host [backup_file]
```

Argument | Required |Description
--- | --- | ---
host | ✓ | The host to connect to. If set to "localhost", then a remote connection will not be attempted.
backup_file | | The optional file from which to read the backup data. If not specified, then the backup data will be read from stdin

