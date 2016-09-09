# Nova

Note: provides the meat and the potatoes of openstack - and that's the instances/virtual machines


## Libvirt (Qemu/KVM)
## Hyper-V
## VMWare
## XenServer
## LXD
## Bare Metal

Note: multiple different backends are readily supported. However, based on some reports, KVM is the hypervisor of choice in 90% of deployments.


## Create
## Delete
## Snapshot
## (Live) Migration
## Evacuate
## Rebuild
## Attach Storage
## Attach Network
## Associate IP

Note: defines consistent primitives for how to handle the virtual instances. Various types of primitives and how they apply


![Nova Architecture](images/nova-architecture.svg)

Note: Nova is really the central point of the OpenStack cloud for typical deployments. Its the core piece that interacts with the various peripheral pieces (e.g. I need an instance, which requires creating a port in neutron, downloading images from glance, creating and attaching bock volumes etc).
