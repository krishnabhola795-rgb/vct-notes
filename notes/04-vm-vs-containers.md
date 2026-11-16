# 4. Virtual Machines vs Containers

- **VM**: has a full guest OS. Heavy (GBs). Starts in minutes.
- **Container**: shares the host OS kernel. Light (MBs). Starts in seconds.

| Point | VM | Container |
|---|---|---|
| Has own OS | Yes | No (shares host kernel) |
| Size | GBs | MBs |
| Start time | Minutes | Seconds |
| Isolation | Strong | Lighter |
| Tool | VMware, VirtualBox | Docker, Podman |
| Best for | Different OS, strong security | Microservices, fast deploy |

## Layers
```
VM:         App -> Guest OS -> Hypervisor -> Hardware
Container:  App -> Container Engine -> Host OS -> Hardware
```

## Which to use?
- Need Linux and Windows on one machine: **VM**.
- Need fast, small, repeatable app deploy: **Container**.
- Many companies use both: containers running inside VMs.
