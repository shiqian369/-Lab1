# -Lab1
1. Check and Enable Virtualization Technology
To Check: On Windows, open Task Manager (Ctrl+Shift+Esc), go to the "Performance" tab, and look for "Virtualization" at the bottom-right. It will say "Enabled" or "Disabled". On Linux, you can run the command: grep -Eoc '(vmx|svm)' /proc/cpuinfo. A value of 1 or higher means it's supported.

To Enable: Reboot your computer and enter the BIOS/UEFI settings (typically by pressing F2, Del, F10, or Esc during boot). Navigate to a menu often called "Advanced," "CPU Configuration," or "Security." Look for an option named "Intel Virtualization Technology (VT-x)," "AMD-V," "SVM Mode," or simply "Virtualization." Enable it, save changes, and exit.

2. The Cloud: Success, Pros, and Cons
Fundamental Reasons for Success:

Economic Efficiency (OpEx vs. CapEx): Companies can avoid large upfront capital expenses (CapEx) on hardware and instead pay only for what they use as an operational expense (OpEx).

Scalability and Elasticity: Resources can be scaled up or down instantly to meet demand, which is impossible with physical hardware.

Ease of Access and Global Reach: Services and data are accessible from anywhere with an internet connection, enabling remote work and global deployment.

Three Pros:

Cost Savings: Reduces the need for purchasing, maintaining, and powering physical servers.

Agility and Speed: Developers can provision resources in minutes, drastically speeding up development and deployment.

Reliability and Disaster Recovery: Cloud providers offer robust data backup and recovery solutions across geographically dispersed data centers.

Three Cons:

Security and Compliance: Storing sensitive data on third-party servers raises concerns about data privacy, regulatory compliance, and potential breaches.

Vendor Lock-in: Migrating services and data from one cloud provider to another can be difficult and expensive due to proprietary technologies.

Potential for Unexpected Costs: Without careful management, usage can spiral, leading to higher-than-expected bills ("bill shock").

3. Primary Function of a Hypervisor
The primary function of a hypervisor (or Virtual Machine Monitor) is to create, run, and manage virtual machines (VMs). It abstracts the physical hardware (CPU, memory, storage, networking) and allocates these resources to one or more guest operating systems.

4. Virtual Machine (VM) and its Benefits
What it is: A Virtual Machine (VM) is a software-based emulation of a physical computer. It runs its own operating system (guest OS) and applications as if it were a separate physical machine, but it shares the resources of a single host computer.

Benefits:

Isolation: VMs are isolated from each other and the host, improving security and stability.

Consolidation: Multiple VMs run on a single physical server, maximizing hardware utilization.

Portability: VMs can be easily moved between different physical hosts.

Legacy Application Support: Can run older operating systems and software on modern hardware.

Testing and Development: Provides safe, isolated sandboxes for testing software and configurations.

5. Use Cases of Virtual Machines
Server Consolidation: Running multiple server workloads (web, database, file) on a single physical machine.

Development and Testing Environments: Creating isolated, disposable environments to build and test new software without affecting production systems.

Running Incompatible Software: Using software designed for an older operating system (e.g., Windows XP) on a modern machine.

Sandboxing for Security: Analyzing malware or browsing the web in a contained VM to protect the host system from infection.

Disaster Recovery: Backing up entire systems as VM images that can be quickly spun up on alternate hardware in case of a failure.

7. In virtualization, what is the guest operating system?
b) The operating system installed on a virtual machine.

8. What does virtual machine isolation mean?
c) Virtual machines run independently and are isolated from each other and the host system.

9. What is the benefit of virtual machine portability?
c) It allows virtual machines to be moved between different physical machines with compatible hypervisors.

10. What is cloning a virtual machine?
Cloning a virtual machine is the process of creating an identical copy of an existing VM. This includes its OS, installed applications, and current state. It is extremely useful for rapidly deploying multiple identical environments (e.g., for a classroom lab or a web server farm) from a single, configured "golden image."
