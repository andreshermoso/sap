#
### [Red Hat Enterprise Linux 9.6 (Plow) 5.14.0-570.12.1.el9_6.x86_64 #1 SMP PREEMPT_DYNAMIC](https://github.com/andreshermoso/sap/tree/main/sap-ase-16-install-rhel/sap-ase-161-install-rhel9)

Errors when installing SAP Adaptive Server Enterprise (ASE) on Red Hat 9.6 (Plow) related to
- the installer
- Java Virtual Machine
- missing libraries
- during the "Configure Historical Monitoring Data Repository" step
- errors during server build
- failures related to specific library files

#
|setup.bin|ERROR|
|:--------|:----|
|ASE_Suite.log|SYSAMWriteLicenseAction.install() Unexpected Fatal Error:|
||UnsatisfiedLinkError: archives/sylapi/libsylapij.so|
||__libnsl.so.2__: cannot open shared object file: No such file or directory|

#
Indicates ASE installer is attempting to load the __libnsl.so.2__ library, but the system cannot locate it.
__libnsl__ provides the Network Services Library (relying on NIS)

