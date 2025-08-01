##
##### root#>
    source ./sa_config.sh

##
##### PATH to locate SQL Anywhere executables and libraries
    /root/sqlanywhere16/bin64/jre170/bin/:/root/sqlanywhere16/bin64:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin

##
##### SQLANY16 points to the installation directory of SQL Anywhere 16 LD_LIBRARY_PATH
    /root/sqlanywhere16

##
##### LD_LIBRARY_PATH specifies the location of shared libraries (i.e ODBC driver libraries)
    /root/sqlanywhere16/lib64:/root/sqlanywhere16/bin64/jre170/lib/amd64/client:/root/sqlanywhere16/bin64/jre170/lib/amd64/server:/root/sqlanywhere16/bin64/jre170/lib/amd64:/root/sqlanywhere16/bin64/jre170/lib/amd64/native_threads:

##
##### DYLD_LIBRARY_PATH (Max OS X)

##
##### ODBCINI points to the location of the odbc.ini file, which contains Data Source Name (DSN) entries


| Database           |
|:-------------------|
| information_schema |
| mysql              |
| performance_schema |
| __sftpgo__         |
8 rows in set (0.00 sec)

mysql> quit
##
# root#
    chown -R sftpgo:sftpgo /etc/sftpgo
    systemctl restart sftpgo.service
    vi /etc/sftpgo/sftpd.log
    
__starting SFTPGo 2.6.6-6825db76-2025-02-24T18:53:31Z__

SFTPD:Bindings:__Address: Port:2022__

__Driver:mysql Name:sftpgo Host:1555.4230.9176.444 Port:3306 Username:sftpgo Password:[redacted]__

__"sender":"dataprovider_mysql","message":"creating initial database schema, version 28"__
##
# mysql>
    use sftpgo;
Database changed

    show tables;


| Tables_in_sftpgo       |
|:-----------------------|
| active_transfers       |
| admins                 |
| admins_groups_mapping  |
| api_keys               |
| configurations         |
| defender_events        |
| defender_hosts         |
| events_actions         |
| events_rules           |
| folders                |
| groups                 |
| groups_folders_mapping |
| ip_lists               |
| nodes                  |
| roles                  |
| rules_actions_mapping  |
| schema_version         |
| shared_sessions        |
| shares                 |
| tasks                  |
| users                  |
| users_folders_mapping  |
| users_groups_mapping   |

    

