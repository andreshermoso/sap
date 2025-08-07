#
### [Red Hat Enterprise Linux 9.6 (Plow) 5.14.0-570.12.1.el9_6.x86_64 #1 SMP PREEMPT_DYNAMIC](https://github.com/andreshermoso/sap/tree/main/sap-ase-16-install-rhel/sap-ase-161-install-rhel9)

Errors when installing SAP Adaptive Server Enterprise (ASE) on Red Hat 9.6 (Plow) related to
- the installer
- Java Virtual Machine
- missing libraries __$${§}$$__
- during the "Configure Historical Monitoring Data Repository" step
- errors during server build
- failures related to specific library files

#
__$${§}$$__ Indicates ASE installer is attempting to load the __libnsl.so.2__ library, but the system cannot locate it.
__libnsl__ provides the Network Services Library (relying on NIS)

|setup.bin|ERROR|
|:--------|:----|
|ASE_Suite.log|SYSAMWriteLicenseAction.install() Unexpected Fatal Error:|
||UnsatisfiedLinkError: archives/sylapi/libsylapij.so|
||__libnsl.so.2__: cannot open shared object file: No such file or directory|

#  
    dnf install libnsl
Last metadata expiration check: 1:05:54 ago on Thu 07 Aug 2025 01:44:19 AM EST.
|Package|Architecture|Version|Repository|Size|
|:-|:-|:-|:-|:-|
|Installing|||||
|libnsl|x86_64|2.34-168.el9|InstallMedia-BaseOS|64 k|
|Transaction Summary|||||
|Install 1 Package|||||
|Installing       : libnsl-2.34-168.el9.x86_64||||1/1|
|Running scriptlet: libnsl-2.34-168.el9.x86_64||||1/1|
|Verifying        : libnsl-2.34-168.el9.x86_64||||1/1|
|Installed products updated.|||||
|Installed:|||||
|libnsl-2.34-168.el9.x86_64|||||
    find / -name *libnsl* -print
__/usr/lib64/libnsl.so.1__

    ln -s libnsl.so.1 libnsl.so.2
    ls -l libnsl.so.2

__lrwxrwxrwx. 1 root root 11 Aug  7 02:54 libnsl.so.2 -> libnsl.so.1__

