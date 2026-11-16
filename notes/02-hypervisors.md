# 2. Hypervisors

**Hypervisor** (also called VMM, Virtual Machine Monitor) = software layer that shares the real hardware between VMs.

## Type 1 - Bare Metal
Runs **directly on hardware**. No normal OS below it.
- Fast and secure. Used in data centers.
- Examples: VMware ESXi, Microsoft Hyper-V, Xen, KVM.

## Type 2 - Hosted
Runs **on top of a normal OS** (like Windows) as an app.
- Easy to install. Slower. Used for learning and testing.
- Examples: VirtualBox, VMware Workstation.

| Point | Type 1 | Type 2 |
|---|---|---|
| Runs on | Hardware | Host OS |
| Speed | Faster | Slower |
| Use | Servers, cloud | Personal, testing |
| Example | ESXi, KVM | VirtualBox |

## What the hypervisor does
1. Divides CPU, RAM, disk, network between VMs.
2. Keeps VMs **isolated** (one VM cannot touch another).
3. Starts, stops, pauses, and snapshots VMs.

## Techniques
- **Full virtualization**: guest OS does not know it is virtual. No change needed.
- **Paravirtualization**: guest OS knows it is virtual and works with the hypervisor. Faster.
- **Hardware-assisted**: CPU helps (Intel VT-x, AMD-V).
