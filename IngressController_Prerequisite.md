## IAM OIDC Connector Configuration.
OIDC is connector is required for controllers (ALB, Nginx etc) to connect with AWS service via Loader and run service on EKS Cluster.
Check if OIDC is available
``` aws iam list-open-id-connect-providers | grep $oidc_id | cut -d "/" -f4\n ```
IF Not then run below command
```eksctl utils associate-iam-oidc-provider --cluster my-cluster --approve```
