# 7. Benefits and Challenges

## Benefits
- Lower cost (fewer physical machines).
- Better hardware use.
- Fast setup of new servers.
- Easy backup, snapshot, and recovery.
- Isolation: a crash in one VM does not stop others.
- Good for testing and learning.
- Less power and space.

## Challenges
- **Performance overhead**: a little slower than real hardware.
- **Single point of failure**: if the host dies, all its VMs stop.
- **VM sprawl**: too many VMs become hard to manage.
- **Security**: a hypervisor attack can affect all VMs.
- **Licensing cost** of some tools.
- Needs skilled people to manage.

## Live migration
Moving a running VM from one host to another with almost no downtime (example: VMware vMotion).
