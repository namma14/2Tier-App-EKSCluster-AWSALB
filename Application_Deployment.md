# Game Application
## Create Farget Profile
We are creating a farget profile to create a new namespace for Game App deployment.
'''
eksctl create fargetprofile \
--cluster my-cluster \
--region us-east-1 \
--name alb-sample-app \
--namespace game-2048
'''
## Deploy the Application Deployment, Service and Ingress YML files.
