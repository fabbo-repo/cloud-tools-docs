### Initialize account and project in gcloud sdk (also used to create a new configuration)
~~~
gcloud init
~~~

### Use a service account with SDK
~~~
gcloud auth activate-service-account --key-file credentials.json
~~~

### Configured accounts
~~~
gcloud auth list
~~~

### Check settings
~~~
gcloud config list
~~~

### Check configuration history
~~~
gcloud config configurations list
~~~

### Activate a configuration
~~~
gcloud config configurations activate <NAME>
~~~

### Delete a configuration (before doing it another configuration must be activated)
~~~
gcloud config configurations delete <NAME>
~~~

### Check projects associated with the configured account
~~~
gcloud projects list
~~~

### Check installed components/modules
~~~
gcloud components list
~~~

