##
##### <img width="22" height="40" align="left" alt="ANY" src="https://help.sap.com/doc/sqlany/1.0/en-US/thumbnails/3362971494/engine128.png" /> [starting point for topics around SQL Anywhere](https://help.sap.com/docs/SUPPORT_CONTENT/sqlany/3362971493.html) 

##
##### root#>
    source ./sa_config.sh

##
##### PATH to locate SQL Anywhere executables and libraries
    /root/sqlanywhere16/bin64/jre170/bin/:/root/sqlanywhere16/bin64:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin

##
##### SQLANY16 points to the installation directory of SQL Anywhere 16
    /root/sqlanywhere16

##
##### LD_LIBRARY_PATH specifies the location of shared libraries (i.e ODBC driver libraries)
    /root/sqlanywhere16/lib64:/root/sqlanywhere16/bin64/jre170/lib/amd64/client:/root/sqlanywhere16/bin64/jre170/lib/amd64/server:/root/sqlanywhere16/bin64/jre170/lib/amd64:/root/sqlanywhere16/bin64/jre170/lib/amd64/native_threads:

##
##### DYLD_LIBRARY_PATH (Max OS X)

##
##### ODBCINI points to the location of the odbc.ini file, which contains Data Source Name (DSN) entries

##
##### root#>
    dbsrv16 -n name the database server -ze (to display server environment variables) {database [options]}*
    dbsrv16 -n demo -ze demo.db

##
 
### SQL Anywhere Network Server Version 16.0.0.2043
### Developer edition, not licensed for deployment.

#### Copyright (c) 2014 SAP AG or an SAP affiliate company.
#### All rights reserved.
#### Use of this software is governed by the Sybase License Agreement.
#### Refer to http://www.sybase.com/softwarelicenses.

##### Connection limit (licensed seats): 3
###### Processors detected: 1 (containing 4 logical processors)
###### Maximum number of processors the server will use: 1 physical processor(s), 2 core(s)
###### This server is licensed to:
######    Developer Edition
######    Restricted Use
###### Running Linux 5.0.0-23-generic #24~18.04.1-Ubuntu SMP Mon Jul 29 16:12:28 UTC 2019 on X86_64
###### Server built for X86_64 processor architecture
###### Direct IO disabled for file '/root/sqlanywhere16/demo.db' because the file system on which it resides does not support it
###### 15824K of memory used for caching
###### Minimum cache size: 15824K, maximum cache size: 14696416K
###### Using a maximum page size of 4096 bytes
###### Multiprogramming level: minimum:4, current:20, maximum:80
###### Automatic tuning of multiprogramming level is enabled
###### Starting database "demo" (/root/sqlanywhere16/demo.db) at Fri Aug 01 2025 22:13
###### Direct IO disabled for file '/root/sqlanywhere16/demo.db' because the file system on which it resides does not support it
###### Transaction log: demo.log
###### Starting checkpoint of "demo" (demo.db) at Fri Aug 01 2025 22:13
###### Finished checkpoint of "demo" (demo.db) at Fri Aug 01 2025 22:13
###### Database "demo" (demo.db) started at Fri Aug 01 2025 22:13
###### Database server started at Fri Aug 01 2025 22:13
###### Trying to start SharedMemory link ...
######     SharedMemory link started successfully
###### Trying to start TCPIP link ...
###### Starting on port 2638
######     TCPIP link started successfully
###### Now accepting requests
###### Press 'q' to shut down the database server

#

-   #### ENV
      - __SQLANY16__  /root/sqlanywhere16
      - __PATH__  /root/sqlanywhere16/bin64/jre170/bin/:/root/sqlanywhere16/bin64:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin
      - __LD_LIBRARY_PATH__  /root/sqlanywhere16/lib64:/root/sqlanywhere16/bin64/jre170/lib/amd64/client:/root/sqlanywhere16/bin64/jre170/lib/amd64/server:/root/sqlanywhere16/bin64/jre170/lib/amd64:/root/sqlanywhere16/bin64/jre170/lib/amd64/native_threads:
      - __JAVA_HOME__  /root/sqlanywhere16/bin64/jre170
      - __SQLANYSAMP16__  /root/sqlanywhere16/samples


#

|DATABASE|TABLE ID|TABLE PAGES|%used|% of file|TABLE NAME|
|:------:|:------:|:---------:|:---:|:-------:|:--:|
|demo|    738|         4  ( 71)|         2  ( 45)|      0|    Customers|
||    739|         2  ( 67)|         2  ( 13)|      0|    Contacts|
||    740|         6  ( 86)|         6  ( 37)|      1|    SalesOrders|
||    741|         7  ( 88)|        11  ( 62)|      2|    SalesOrderItems|
||    742|        20  ( 91)|         5  ( 10)|      3|    Products|
||    743|         1  (  5)|         1  (  9)|      0|    FinancialCodes|
||    744|         1  ( 43)|         2  ( 25)|      0|    FinancialData|
||    745|         1  (  3)|         2  (  9)|      0|    Departments|
||    746|         3  ( 71)|         3  ( 27)|      0|    Employees|
||    747|         2  ( 51)|         2  (  9)|      0|    MarketingInformation|
||    748|         3  ( 68)|         1  ( 12)|      0|    SpatialContacts|
||    749|         2  ( 64)|         1  ( 10)|      0|    SpatialShapes|
#

