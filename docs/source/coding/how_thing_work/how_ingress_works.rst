How Ingress Works
===================================

**How Application Load Balance Ingress Works**

Ingress is a Kubernetes object that allows you to manage external or internal HTTP(S) access to services running in your Kubernetes cluster. It can be used to route requests for different paths to different services.

**AWS ALB Ingress Controller**

The AWS ALB Ingress controller is an open-source project that automates the creation and configuration of ALBs for Kubernetes Ingress resources. It can help simplify and automate the management of your Ingress resources.

- Open-source project that automates the creation and configuration of ALBs for Kubernetes Ingress resources.
- Compatible with any Kubernetes cluster, including EKS.
- Listens for Ingress resources in your Kubernetes cluster.
- Creates an ALB and configures it to route traffic to the targets specified in the Ingress resource.
- Can also automatically distribute traffic across multiple ALBs.

**Key Features of AWS Load Balancer Controller**

- **Sharing ALBs**: You can use one ALB for multiple Ingress resources.
- **Support for NLBs**: NLBs are good for high-traffic apps.
- **Support for TargetGroupBinding**: Bind services to ELB target groups.
- **Support for fully private clusters**: Keep clusters isolated from the internet.

**How Ingress Works**

Ingress works by defining a set of rules that map incoming requests to specific services. These rules can be based on the hostname, path, or other criteria.
When a request arrives at your Kubernetes cluster, the Ingress controller will use these rules to determine which service to route the request to.

For example:
- Requests for `www.ntechdeveloper.com/app1` could be routed to a service called `app1`.
- Requests for `www.ntechdeveloper.com/app2` could be routed to a service called `app2`.
- Requests for `www.ntechdeveloper.com/user` could be routed to a service called `user`.

Ingress is a powerful tool that can help simplify and manage the routing of external traffic to your Kubernetes services. If you are running a Kubernetes cluster, consider using Ingress.
