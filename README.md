# Proxmox Homelab Infrastructure

## Objective

This project focused on designing and operating a self-hosted virtualization platform using Proxmox VE to support multiple application stacks and cybersecurity projects.
The goal was to build a flexible, low-overhead environment capable of running isolated workloads while maintaining strong operational control, scalability, and security awareness.

The environment serves as a foundational platform for hosting containerized workloads and future security labs, while demonstrating practical experience with virtualization, containerization, and system architecture.

### Skills Learned

 - Practical experience with enterprise-style virtualization using Proxmox VE
 - Understanding of workload isolation using LXC containers versus full virtual machines
 - Resource management and capacity planning (CPU, memory, storage)
 - Designing infrastructure to support multiple independent projects
 - Evaluating security and performance tradeoffs in virtualization choices
 - Operational mindset for maintaining long-running infrastructure

### Tools Used

 - Proxmox VE – Hypervisor and virtualization management
 - LXC (Linux Containers) – Lightweight containerized workloads
 - Linux-based operating systems (Ubuntu/Debian)
 - Web-based management interfaces and CLI tools

## Steps

The following artifacts document the operational state and architectural decisions of the Proxmox-based infrastructure. Screenshots are selected to demonstrate system design, workload isolation, and real-world operation rather than step-by-step configuration.

### Ref 1: Proxmox Datacenter Overview


<img width="1512" height="822" alt="Screenshot 2026-01-31 at 3 44 22 PM" src="https://github.com/user-attachments/assets/c00573fb-9fa0-4e61-b3af-efc6bc423e6b" />

This screenshot shows the Proxmox VE datacenter summary view, providing a high-level overview of the virtualization environment. It highlights the operational health of the platform, active nodes, and guest workloads, along with real-time resource utilization across CPU, memory, and storage. This view demonstrates centralized infrastructure management and confirms the system is operating as a stable foundation for hosting multiple isolated projects.


### Ref 2: Host Node Summary (Resource Utilization)

<img width="1512" height="822" alt="Screenshot 2026-01-31 at 3 52 42 PM" src="https://github.com/user-attachments/assets/8d47e6e8-e06a-4d3d-bb80-c4fd913d7bb7" />

This screenshot shows the summary view of the Proxmox host node, displaying real-time CPU, memory, storage, and uptime metrics. It demonstrates active monitoring of host-level resources and confirms the system is operating within expected utilization ranges while supporting containerized workloads. This view reflects an operational focus on performance, stability, and capacity planning at the infrastructure level.


### Ref 3: LXC Container Summary (Application Host)
![Screensho](https://github.com/user-attachments/assets/e4c764ee-ff4f-4e7c-a899-818f7a462c6f)

This screenshot shows the summary view of an unprivileged LXC container running on the Proxmox host and serving as a dedicated environment for application workloads. It highlights the container’s running state, uptime, and resource utilization, demonstrating lightweight isolation and controlled resource usage as an alternative to full virtual machines.

