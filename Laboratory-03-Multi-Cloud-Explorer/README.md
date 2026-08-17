# Linux Server Investigation
## Operating System

PRETTY_NAME="Ubuntu 24.04.4 LTS"
NAME="Ubuntu"
VERSION_ID="24.04"
VERSION="24.04.4 LTS (Noble Numbat)"
VERSION_CODENAME=noble
ID=ubuntu
ID_LIKE=debian

## CPU Information

Architecture: x86_64
CPU(s): 1
Vendor ID: GenuineIntel
Model name: Intel Xeon E312xx (Sandy Bridge, IBRS update)
Thread(s) per core: 1
Core(s) per socket: 1
Socket(s): 1
Virtualization type: full (KVM)

## Memory
          total        used        free      shared  buff/cache   available

Mem: 1.9Gi 412Mi 842Mi 1.1Mi 816Mi 1.5Gi
Swap: 1.0Gi 0B 1.0Gi

## Disk Space

Filesystem Size Used Avail Use% Mounted on
tmpfs 191M 996K 190M 1% /run
/dev/vda1 19G 5.4G 13G 30% /
tmpfs 952M 84K 952M 1% /dev/shm
tmpfs 5.0M 0 5.0M 0% /run/lock
/dev/vda16 881M 117M 703M 15% /boot
/dev/vda15 105M 6.2M 99M 6% /boot/efi

## Cloud Migration Analysis
**If this Linux server were migrated to the cloud, which AWS, Azure, and GCP services could host it?**
Given this server's small footprint — a single vCPU, about 2 GB of RAM, and roughly 19 GB of disk — it maps well to the smallest, burstable-performance instance tiers on each platform rather than dedicated high-compute options. On AWS, this would run comfortably on an **Amazon EC2 t3.micro** or **t2.micro** instance, which are built for low, steady workloads with occasional bursts. On Microsoft Azure, the equivalent is the **B1s Burstable VM**, designed for the same kind of light, non-continuous usage pattern. On Google Cloud Platform, this server would map to an **e2-micro** or **e2-small** Compute Engine instance. For storage, the server's ~19 GB disk would be backed by a small **Amazon EBS** volume on AWS, an **Azure Managed Disk** on Azure, or a **Persistent Disk** on GCP — all sized around 20–30 GB to leave headroom for growth.
