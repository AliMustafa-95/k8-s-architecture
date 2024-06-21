Master Node Components
1. API Server

Acts as the frontend for the Kubernetes control plane. It exposes the Kubernetes API.

2. Scheduler

Assigns nodes to newly created pods. It watches for unscheduled pods and finds the best node for them to run on.

3. ETCD

A distributed key-value store used for storing all cluster data, including the configuration, state, and metadata.

4. Controller Manager

Runs various controllers that regulate the state of the cluster, ensuring the cluster is in the desired state. Examples include the node controller, replication controller, and endpoint controller.

5. Cloud Controller Manager

Manages cloud-specific control logic, allowing for integration with various cloud providers. It enables the cluster to interact with the underlying cloud infrastructure.

Worker Node Components

6. Kubelet

An agent that runs on each node in the cluster. It ensures that containers are running in a pod. It communicates with the master node to receive commands and report the status.

7. Kube Proxy

Maintains network rules on nodes, allowing for network communication to your pods. It handles forwarding traffic and manages IP addresses.

8. Container Runtime

The software responsible for running containers. Common examples include Docker, containerd, and CRI-O.