 I do not have own aws, so I have done this task with VirtualBox + Vagrant

- We need to create HA csv parser application which will process data file and write it to the RDMS. 
  Service needs to run two different availibility zone at the same time.


+  Create a small multi AZ Kubernetes cluster on AWS which will accommodate all components.
+ Create an applicaton which is will process data file which provided as attachment with this case study (columns: sku, name, price) insert to the db (rds is a plus),
+ save uploaded files in persistent storage
+ create a simple web interface which will show all processed files
+ add action buttons for each row (archive, delete, etc.)

Gitlab has been replaced by Jenkins

+ Create Gitlab instance in Kubernetes cluster and then deploy the csv parser application with Gitlab ci.
 -/+ (just need to set hook) Every changes on gitlab repos should be deployed to the target nodes.
 - Support accessible feature branch deployments via CI.
    Please create a diagram to explain this architecture.
    Also;
    - Route 53 is a plus
    - Ansible is a plus
    - CloudFront for CDN is a plus
