# Overview
Cilium is an open source project to provide networking, security, and observability for cloud native environments such as Kubernetes clusters and other container orchestration platforms.

At the foundation of Cilium is a new Linux kernel technology called eBPF, which enables the dynamic insertion of powerful security, visibility, and networking control logic into the Linux kernel. eBPF is used to provide high-performance networking, multi-cluster and multi-cloud capabilities, advanced load balancing, transparent encryption, extensive network security capabilities, transparent observability, and much more.

Cilium comprises four key components: the Cilium agent, the Cilium client command line tool, the Cilium operator, and the Cilium CNI plugin. The agent, running on all cluster nodes, configures networking, load balancing, policies, and monitoring via Kubernetes or APIs that describe networking, service load-balancing, network policies, and visibility & monitoring requirements.

The client tool, bundled with the agent, inspects and manages the local agent's status, offering direct access to eBPF maps. The operator centrally manages cluster tasks, handling them collectively rather than per node. The CNI plugin, invoked by Kubernetes during pod scheduling or termination, interacts with the node's Cilium API to configure necessary datapaths for networking, load balancing, and network policies.
