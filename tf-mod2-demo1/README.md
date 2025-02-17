# Terraform Demo

Creates a VPC, subnet, firewall rules, and a VM.  

![Diagram](mod2-demo1.png)


## Modify
In provider.tf, change the two locations which say FILL-IN.  The first points to the json file that was downloaded when creating a service account.  The second is the project name.

In main.tf, update the firewall resource where it says FILL-IN to match your GCP project name. Or, you can simply delete that line and it will use the project name defined in provider.tf.

## To Run
```
terraform init
terraform plan
terraform apply
```

## Debugging / Visualizing
You can use terraform show to output the current infrastructure (that's been deployed with terraform).  You can output in json, which can be useful.

```
terraform show -json | jq
```

## Google Cloud
Log into Google Cloud Platform, and see that it created 

## To Delete
```
terraform destroy
```
