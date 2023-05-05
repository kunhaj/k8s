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
