We can create EKS cluster from CLI and AWS Interface
# AWS CLI:
command: eksctl create cluster --name my-cluster --region us-east-1 -- fargate
- name: Cluster Name
- Region: Region in which we would like to create cluster
- Fargate: Similar to worker nodes.Allows to run containers without having to manage control plane or Data plane.
Fargate profile get created with Default and Kube-system namespaces if we need to create a different namespace then we would need to create
a new fargate profile. Fargate option is available : EKS cluster > Compute > Scroll down to Faragte
