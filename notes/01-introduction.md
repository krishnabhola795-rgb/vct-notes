# 1. Introduction to Virtualization

**Virtualization** = making a virtual (software-based) version of something real, like a computer, storage, or network.

## Simple example
One physical computer can run many "virtual computers". Each one acts like a separate machine with its own OS and apps.

## Key words
- **Host**: the real physical machine.
- **Guest**: the virtual machine running on the host.
- **Virtual Machine (VM)**: a software computer inside a real computer.
- **Hypervisor**: software that creates and manages VMs.
- **Resource pooling**: sharing CPU, RAM, and disk between many VMs.

## Why we need it
- Real servers are often only 10-20% used. Virtualization uses the rest.
- Saves money (fewer machines, less power).
- Easy to copy, move, and back up.

## Short history
- 1960s: IBM first used it on mainframes.
- 1999: VMware made it popular on normal PCs.
- 2000s onward: Xen, KVM, Hyper-V, then cloud and containers.
