# k8s
kubernetes notes

1. `kubectl get`: This command is used to retrieve information about resources in a Kubernetes cluster. 
For example, you can use `kubectl get pods` to get a list of all the pods in the cluster.

2. `kubectl describe`: This command is used to get more detailed information about a specific resource. 
For example, you can use `kubectl describe pod <pod-name>` to get detailed information about a specific pod.

3. `kubectl apply`: This command is used to apply a configuration file to the cluster. 
For example, you can use `kubectl apply -f deployment.yaml` to apply a deployment configuration to the cluster.

4. `kubectl delete`: This command is used to delete resources from the cluster. 
For example, you can use `kubectl delete pod <pod-name>` to delete a specific pod.

5. `kubectl logs`: This command is used to view the logs of a container running in a pod. 
For example, you can use `kubectl logs <pod-name>` to view the logs of the first container in a pod.

6. `kubectl exec`: This command is used to execute a command in a container running in a pod. 
For example, you can use `kubectl exec <pod-name> -- <command>` to execute a command in the first container in a pod.

7. `kubectl port-forward`: This command is used to forward a port from a pod to your local machine. 
For example, you can use `kubectl port-forward <pod-name> <local-port>:<pod-port>` to forward port 80 from a pod to port 8080 on your local machine.

8. `kubectl create`: This command is used to create resources in the cluster. 
For example, you can use `kubectl create deployment <deployment-name> --image=<image-name>` to create a new deployment in the cluster.

9. `kubectl scale`: This command is used to scale resources in the cluster. 
For example, you can use `kubectl scale deployment <deployment-name> --replicas=<number-of-replicas>` to scale a deployment to a specific number of replicas.

`kubectl --help` or `kubectl <command> --help` for help on specific commands.

#### `kubectl get`

1. `kubectl get pods`: This command is used to get a list of all the pods running in a cluster, along with their current status, age, IP address, and node name.

2. `kubectl get nodes`: This command is used to get a list of all the nodes in the cluster, along with their current status, age, IP address, and number of pods running on each node.

3. `kubectl get services`: This command is used to get a list of all the services in the cluster, along with their current status, age, IP address, and port mappings.

4. `kubectl get deployments`: This command is used to get a list of all the deployments in the cluster, along with their current status, age, number of replicas, and available updates.

5. `kubectl get replicasets`: This command is used to get a list of all the replicasets in the cluster, along with their current status, age, and number of replicas.

6. `kubectl get configmaps`: This command is used to get a list of all the configmaps in the cluster, along with their current status, age, and data.

7. `kubectl get secrets`: This command is used to get a list of all the secrets in the cluster, along with their current status, age, and data.

8. `kubectl get persistentvolumes`: This command is used to get a list of all the persistent volumes in the cluster, along with their current status, age, storage class, and capacity.

9. `kubectl get persistentvolumeclaims`: This command is used to get a list of all the persistent volume claims in the cluster, along with their current status, age, storage class, and capacity.

10. `kubectl get namespaces`: This command is used to get a list of all the namespaces in the cluster, along with their current status, age, and labels.

For more information, you can refer to the official Kubernetes documentation or run `kubectl get --help` for help on specific commands.
