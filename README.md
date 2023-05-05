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

#### `kubectl describe`


1. `kubectl describe pods`: This command is used to get detailed information about all the pods running in a cluster, including their status, IP address, labels, annotations, and events.

2. `kubectl describe nodes`: This command is used to get detailed information about all the nodes in the cluster, including their status, capacity, allocatable resources, labels, and annotations.

3. `kubectl describe services`: This command is used to get detailed information about all the services in the cluster, including their type, IP address, port mappings, labels, and annotations.

4. `kubectl describe deployments`: This command is used to get detailed information about all the deployments in the cluster, including their status, replicas, strategy, labels, annotations, and events.

5. `kubectl describe replicasets`: This command is used to get detailed information about all the replicasets in the cluster, including their status, number of replicas, labels, and annotations.

6. `kubectl describe configmaps`: This command is used to get detailed information about all the configmaps in the cluster, including their data, labels, and annotations.

7. `kubectl describe secrets`: This command is used to get detailed information about all the secrets in the cluster, including their data, type, and labels.

8. `kubectl describe persistentvolumes`: This command is used to get detailed information about all the persistent volumes in the cluster, including their status, capacity, access modes, labels, and annotations.

9. `kubectl describe persistentvolumeclaims`: This command is used to get detailed information about all the persistent volume claims in the cluster, including their status, capacity, access modes, labels, and annotations.

10. `kubectl describe namespaces`: This command is used to get detailed information about all the namespaces in the cluster, including their status, labels, and annotations.

For more information, you can refer to the official Kubernetes documentation or run `kubectl describe --help` for help on specific commands.


#### `kubectl apply`

1. `kubectl apply -f <filename>`: This command is used to create or update Kubernetes resources from a YAML or JSON file. The file can contain one or more Kubernetes objects, such as pods, services, deployments, and more.

2. `kubectl apply -f <directory>`: This command is used to create or update Kubernetes resources from a directory containing YAML or JSON files. The command will apply all the files in the directory in alphabetical order.

3. `kubectl apply -f <url>`: This command is used to create or update Kubernetes resources from a URL that points to a YAML or JSON file.

4. `kubectl apply -k <directory>`: This command is used to create or update Kubernetes resources from a directory containing YAML files that are organized into a hierarchy using kustomization files. This allows you to customize and manage Kubernetes resources using overlays, patches, and environment variables.

5. `kubectl apply -R -f <directory>`: This command is used to create or update Kubernetes resources from a directory and all its subdirectories containing YAML or JSON files.

6. `kubectl apply -f <filename> --prune`: This command is used to create or update Kubernetes resources from a YAML or JSON file and delete any resources that are no longer defined in the file.

For more information, you can refer to the official Kubernetes documentation or run `kubectl apply --help` for help on specific commands.


#### `kubectl logs` 

1. `kubectl logs <pod-name>`: This command is used to display the logs of a pod. By default, it displays the logs from the main container in the pod. You can specify a different container with the `-c` flag, for example `kubectl logs <pod-name> -c <container-name>`.

2. `kubectl logs -f <pod-name>`: This command is used to stream the logs of a pod in real-time. This is useful for debugging and monitoring running applications.

3. `kubectl logs --previous <pod-name>`: This command is used to display the logs of the previous container instance that ran in the pod.

4. `kubectl logs <pod-name> --since=<duration>`: This command is used to display the logs of a pod for a specific duration. The duration can be specified in seconds, minutes, or hours.

5. `kubectl logs <pod-name> --tail=<number>`: This command is used to display the last N lines of logs from a pod, where N is the number specified by the `--tail` flag. By default, it displays the last 10 lines of logs.

6. `kubectl logs <pod-name> -p`: This command is used to display the logs of a pod's previous instance. This is useful when a pod is restarted or when a deployment rolls back to a previous version.

 For more information, you can refer to the official Kubernetes documentation or run `kubectl logs --help` for help on specific commands.
