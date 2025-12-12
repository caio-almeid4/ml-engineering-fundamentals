
### Container x VM

**VM**: Hardware -> Hypervisor -> OS -> App
- Using of unnecessary resources
- Enormous OS for a lightweight application
- Slow initialize

**Container**: Hardware (Server) -> OS (Linux) -> Container Engine (Docker) -> (App, App, App)
* Isolated environment
* Set of linux primitive functionalities (cgroups, chroot, ...)
* All containers share the same Kernel from the host server
* Advantages:
	* Resources optimization
	* Packaging
	* Immutability
	* Easier deploy
	
![[Pasted image 20251211104148.png]]


### Architecture

![[Pasted image 20251211105400.png]]
- Client sends the action
- Host executes it
	- Daemon: background process 
	- Store/download images
	- Create containers
- Registry stores images