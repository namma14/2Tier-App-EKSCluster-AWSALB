# 2Tier-App-EKSCluster-AWSALB
To to debug load balancer if its not running
kubectl edit deploy/aws-load-balancer-controller -n kubec-system
goto status section and check for errors
