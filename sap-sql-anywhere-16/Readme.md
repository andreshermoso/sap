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
##### root#> dbsrv16
##### ...... $${server options}$$ -n name the database server -ze (to display server environment variables) {database [options]}*
