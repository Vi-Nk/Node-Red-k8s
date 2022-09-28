# Node-Red-k8s
Kubernetes configurations for Node Red K8s deployments

## Deployment steps 

The node-red project can be deployed using generic helm charts provided in the repository. Values can be changed as intended.

 ### Helm charts :
    Customization of values as per the environment needs can be done in charts/node-red/values.yaml before executing deployment command. Once customized , below command can be executed to install node-red related artifacts in the k8s system of choice .

    **Note** : The cluster specific fields in values.yaml file are marked with *Required* comment.They have to be populated appropriately before the deployment steps mentioned below.

    `cd charts/node-red`

    `helm install node-red . -n <namespace>`

    After successful deployment , Node red ingress can be accessed from the url mentioned in values.yaml from browsers/UI viewers.
