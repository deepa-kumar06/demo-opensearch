# demo-opensearch

Deployment Steps:

Clone the below repository and apply terraform

s1- git clone https://github.com/deepa-kumar06/demo-opensearch/
s2- terraform apply 

In the ouput, you can see the opensearch cluster deployed in the eks

Note: Please 'terraform destroy' once the output is verified.

Roadmap:

* Running the Operator locally
* Clone the repo and go to the opensearch-operator folder.
* Run make build manifests to build the controller binary and the manifests
* Start a kubernetes cluster and make sure your ~/.kube/config points to it
* Run make install to create the CRD in the kubernetes cluster
* Start the operator by running make run
* Deploy an opensearch cluster.

Current features/Best practice followed:

* Deploy a new OS cluster.
* Ability to deploy multiple clusters.
* Spin up OS dashboards.
* Configuration of all node roles (master, data, coordinating..).
* Scale the cluster resources (manually), per nodes’ role group.
* Drain strategy for scale down.
* Version updates.
* Change nodes’ memory allocation and limits.
* Secured installation features.
* Certificate management.
* Scaling nodes’ disks - increase disk size.
* Cluster configurations and nodes’ settings updates.

Prerequisites:

* Terraform v1.3+ installed locally.
* An AWS account
* the AWS CLI v2.7.0/v1.24.0 or newer, installed and configured using aws configure
* AWS IAM Authenticator
* kubectl v1.24.0 or newer




