# PotatoLab - Personal Homelab

PotatoLab is my long-running homelab project, established in 2015 as a hands-on environment for exploring new technologies and developing skills in networking, systems administration, DevOps, and software development. Over the years, it has undergone multiple iterations and served as a platform for hosting applications, experimenting with infrastructure, and supporting my personal technology needs.

Recently, I have streamlined the environment to reduce hardware complexity and operational overhead while maintaining the capabilities I rely on. This redesign included consolidating server hardware around three primary functions: core infrastructure services (DNS, DHCP, and NTP), home automation, and general-purpose workloads such as self-hosted applications and AI services. I also standardized my network infrastructure on Ubiquiti equipment to simplify centralized management and administration.


## Infrastructure Automation

I use Ansible playbooks to automate the configuration and deployment of much of my homelab infrastructure, reducing repetitive manual tasks and maintaining consistency across the environment.

Key automation workflows include:

* **DNS and DHCP Management**: Configure network services through the Technitium DNS Server API and Cloudflare API, including DNS management for external access and DNS-based Let's Encrypt certificate validation.
* **Virtualization Management**: Provision and manage Proxmox virtual machines (VMs) and Linux containers (LXCs).
* **Server Configuration**: Standardize baseline server configurations, including NTP synchronization, message of the day (MOTD), and other common system settings.
* **Application Deployment**: Deploy and manage containerized applications using Docker Compose, as well as Kubernetes workloads on Talos Linux using kubectl.

PotatoLab continues to serve as a practical environment for building, testing, and refining infrastructure automation, self-hosted services, and new technologies.

## Most Commonly Used Software

The following applications make up the core of my homelab, supporting everything from infrastructure management and software development to home automation and personal services.

- **[Technitium DNS Server](https://technitium.com/)** — Provides DNS and DHCP services for my home network, with built-in ad blocking and API support for automated configuration through Ansible.

- **[Home Assistant](https://www.home-assistant.io/)** — Powers my home automation setup, integrating smart devices and automating everyday tasks. Making life more convenient, one automation at a time.

- **[Immich](https://immich.app/)** — Self-hosted photo and video management for backing up and organizing my personal and family photo libraries.

- **[Gitea](https://about.gitea.com/)** — Hosts my self-managed Git repositories and supports my development workflows, including synchronizing repositories with GitHub.

- **[Mealie](https://mealie.io/)** — Organizes my recipe collection and helps with meal planning and meal preparation.

- **[Ollama](https://ollama.com/)** — Runs AI models locally for general-purpose queries, coding assistance, and personal productivity tasks.

- **Synology NAS** — Provides centralized network storage and local backups for my files and other important data.

## Diagram

[![Homelab_Diagram](/images/diagram.jpg)](/images/diagram.jpg)

## Current Setup

[![Current](/images/current.png)](/images/current.png)

The homelab has undergone significant modernization and infrastructure consolidation. All networking equipment has been replaced with Ubiquiti hardware to simplify network management, and custom-built 2U storage servers have been replaced with Synology systems. The number of Dell PCs has been reduced by consolidating applications into a single-node Kubernetes cluster and Proxmox-hosted LXC containers and virtual machines. Additionally, a custom-built desktop PC (shown on the right) equipped with an NVIDIA GeForce RTX 3090 was added to host Proxmox workloads and AI agents for various use cases.

Hardware List (Top to Bottom, Left to Right):
* Ubiquiti Dream Machine Pro
* Ubiquiti 24-Port 1G Core Switch (US-24)
* Dell Optiplex 7060m MicroDesktop PC running Home Automation system
* GoveeLife Bluetooth Temperature/Humidity Sensor
* 2x Dell Optiplex 7040m MicroDesktop PCs running DNS/DHCP/NTP services
* Synology DS423 (Main Storage)
* Synology DS423+ (Backup Storage)
* CyberPower 1500VA/900W CST150UC2-E UPS
* Custom-Built Desktop PC w/ Nvidia GTX 3090 GPU

Not in Picture:
* Ubiquiti USW-Lite-16-PoE House Switch
* 2x Ubiquiti USW-Flex-Mini Room Switches
* 2x Ubiquiti U7 Lite WAPs

## Previous Setups

### 9th Revision (2025)

**MISSING PHOTO**

Replaced Dell switches with HP.

### 8th Revision (May 2023)

[![8th Revision](/images/8th_revision.png)](/images/8th_revision.png)

Replaced Cisco switches with Dell.

### 7th Revision (Jan 2023)

[![7th Revision](/images/7th_revision.png)](/images/7th_revision.png)

Designed and built a custom enclosed server rack, upgraded network switching from Netgear to Cisco, and replaced 1U Supermicro servers with individual Dell micro desktop PCs to create a more compact, energy-efficient Kubernetes cluster.

### 6th Revision (2022)

[![6th Revision](/images/6th_revision.jpg)](/images/6th_revision.jpg)

Replaced Dell micro desktop PCs with 1U Supermicro rackmount servers to increase server density and transition the Kubernetes cluster to dedicated rackmount hardware.

### 5th Revision (2021)

[![5th Revision](/images/5th_revision.jpg)](/images/5th_revision.jpg)

Replaced Dell network switches with Netgear and MikroTik equipment, migrated workloads from a custom-built 2U server to Dell micro desktop PCs, and replaced ODROID-HC4 devices with custom-built 2U Supermicro storage servers.

### 4th Revision (2019-2020)

[![4th Revision](/images/4th_revision.jpg)](/images/4th_revision.jpg)

Upgraded from a basic college-era setup to a more structured homelab with dedicated hardware for firewall and network services, as well as application hosting, following the transition from college to full-time employment.

### 3rd Revision (2017-2019)

[![3rd Revision](/images/3rd_revision.jpg)](/images/3rd_revision.jpg)

Upgraded server hardware to support the growing infrastructure and computing needs of my homelab during the final years of college.

### 2nd Revision (2016-2017)

Missing

### 1st Revision (2015-2016)

[![1st Revision](/images/1st_revision.jpg)](/images/1st_revision.jpg)

Built my first homelab using repurposed PC hardware from my parents and a secondhand computer purchased from a local electronics reseller.
