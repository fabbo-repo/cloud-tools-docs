### Create a Cloud SQL instance
~~~
gcloud sql instances create <INSTANCE_NAME> --database-version=<DB_VERSION> --cpu=<X> --memory=<Y>GiB --region=<REION> --root-password=<PASSWORD>
~~~

### Delete a Cloud SQL instance
~~~
gcloud sql instances delete <INSTANCE_NAME>
~~~

### Delete Cloud SQL instances
~~~
gcloud sql instances list
~~~

### Create a Database
~~~
gcloud sql databases create <DATABASE_NAME> -i <INSTANCE_NAME>
~~~

### Delete a Database
~~~
gcloud sql databases delete <DATABASE_NAME> -i <INSTANCE_NAME>
~~~

### List Databases
~~~
gcloud sql databases list -i <INSTANCE_NAME>
~~~

### Create a Backup
~~~
gcloud sql backups create -i <INSTANCE_NAME>
~~~

### List Backups
~~~
gcloud sql backups list -i <INSTANCE_NAME>
~~~

### Delete a Backup
~~~
gcloud sql backups delete <BACKUP_ID> -i <INSTANCE_NAME>
~~~

### Restore a Backup to an instance
~~~
gcloud sql backups restore <BACKUP_ID> --restore-instance <INSTANCE_NAME>
~~~
> ***--backup-instance <INSTANCE_NAME>*** must be spcified when the backup instance is different from the restore instance

### Create user
~~~
gcloud sql users create <USERNAME> -i <INSTANCE_NAME> --password <PASSWORD>
~~~

### Delete user
~~~
gcloud sql users delete <USERNAME> -i <INSTANCE_NAME>
~~~

### List users
~~~
gcloud sql users list -i <INSTANCE_NAME>
~~~