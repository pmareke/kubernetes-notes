# Kubernetes notes

## Terminology

- `Node`: A worker machine in Kubernetes, part of a cluster.
- `Cluster`: A set of Nodes that run containerized applications managed by Kubernetes. 
    - For this example, and in most common Kubernetes deployments, nodes in the cluster are not part of the public internet.
- `Edge router`: A router that enforces the firewall policy for your cluster.
    - This could be a gateway managed by a cloud provider or a physical piece of hardware.
- `Cluster network`: A set of links, logical or physical, that facilitate communication within a cluster according to the Kubernetes networking model.
- `Service`: A Kubernetes Service that identifies a set of Pods using label selectors.
    - Unless mentioned otherwise, Services are assumed to have virtual IPs only routable within the cluster network.

## Kubernetes cluster diagram

![Kubernetes cluster](images/cluster.png)

## Concepts

- [Config Maps](concepts/config_maps.md)
- [Containers](concepts/containers.md)
- [Deployments](concepts/deployments.md)
- [Daemon Sets](concepts/daemon_sets.md)
- [Images](concepts/images.md)
- [Ingress](concepts/ingress/main.md)
    - [Classes](concepts/ingress/classes.md)
    - [Controllers](concepts/ingress/controllers.md)
- [Jobs](concepts/jobs.md)
- [Cron Jobs](concepts/cron_jobs.md)
- [Namespaces](concepts/namespaces.md)
- [Nodes](concepts/nodes.md)
- [Pods](concepts/pods.md)
- [Probes](concepts/probes.md)
- [Roles](concepts/roles.md)
- [Roles Bindings](concepts/roles_bindings.md)
- [Secrets](concepts/secrets.md)
- [Services Accounts](concepts/service_accounts.md)
- [Services](concepts/services.md)
- [Stateful Sets](concepts/stateful_sets.md)
- [Volumes](concepts/volumes.md)
