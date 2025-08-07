#
### [Red Hat Enterprise Linux 9.6 (Plow) 5.14.0-570.12.1.el9_6.x86_64 #1 SMP PREEMPT_DYNAMIC](https://github.com/andreshermoso/sap/tree/main/sap-ase-16-install-rhel/sap-ase-161-install-rhel9)

Errors when installing SAP Adaptive Server Enterprise (ASE) on Red Hat 9.6 (Plow) related to
- the installer
- Java Virtual Machine
- missing libraries $${§}$$
- during the "Configure Historical Monitoring Data Repository" step
- errors during server build
- failures related to specific library files

#
$${§}$$ Indicates ASE installer is attempting to load the __libnsl.so.2__ library, but the system cannot locate it.
__libnsl__ provides the Network Services Library (relying on NIS)

|setup.bin|ERROR|
|:--------|:----|
|ASE_Suite.log|SYSAMWriteLicenseAction.install() Unexpected Fatal Error:|
||UnsatisfiedLinkError: archives/sylapi/libsylapij.so|
||__libnsl.so.2__: cannot open shared object file: No such file or directory|

##
##### root#> 
    dnf install libnsl
####### Last metadata expiration check: 1:05:54 ago on Thu 07 Aug 2025 01:44:19 AM EST.
|1|2|
|:-|:-|
|||

Dependencies resolved.
=============================================================================================================================================================
 Package                         Architecture                    Version                                  Repository                                    Size
=============================================================================================================================================================
Installing:
 libnsl                          x86_64                          2.34-168.el9                             InstallMedia-BaseOS                           64 k

Transaction Summary
=============================================================================================================================================================
Install  1 Package

Total size: 64 k
Installed size: 99 k
Is this ok [y/N]: y
Downloading Packages:
Running transaction check
Transaction check succeeded.
Running transaction test
Transaction test succeeded.
Running transaction
  Preparing        :                                                                                                                                     1/1 
  Installing       : libnsl-2.34-168.el9.x86_64                                                                                                          1/1 
  Running scriptlet: libnsl-2.34-168.el9.x86_64                                                                                                          1/1 
  Verifying        : libnsl-2.34-168.el9.x86_64                                                                                                          1/1 
Installed products updated.

Installed:
  libnsl-2.34-168.el9.x86_64                                                                                                                                 

Complete!
##
##### PATH to locate SQL Anywhere executables and libraries
    /root/sqlanywhere16/bin64/jre170/bin/:/root/sqlanywhere16/bin64:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin
