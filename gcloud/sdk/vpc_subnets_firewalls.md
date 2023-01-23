### List VPC networks
~~~
gcloud compute networks list
~~~

### List subnets
~~~
gcloud compute networks subnets list
~~~

### List subnets for a VPC
~~~
gcloud compute networks subnets list --network <VPC_NAME>
~~~

### Create a VPC
~~~
gcloud compute networks create <VPC_NAME> --description "<DESCRIPTION>" 
~~~
> If ***--subnet-mode custom*** is not specified it will create a subnet in each region.

### Create a firewall rule
~~~
gcloud compute firewall-rules create <FIREWALL_NAME> --network <VPC_NAME> --allow tcp:22,tcp:3389,icmp
~~~

### Create a subnet
~~~
gcloud compute networks subnets create <SUBNET_NAME> --network <VPC_NAME> --regions <REGION> --range <IP_ADDR_MASK>
~~~
> **IP_ADDR_MASK** can be *10.10.1.0/24*

### Delete a subnet
~~~
gcloud compute networks subnets delete <SUBNET_NAME> --network <VPC_NAME> --regions <REGION>
~~~

### Delete a firewall rule
~~~
gcloud compute firewall-rules delete <FIREWALL_NAME>
~~~

### Delete a VPC
~~~
gcloud compute networks delete <VPC_NAME>
~~~
