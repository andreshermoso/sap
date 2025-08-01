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
[0] LD_LIBRARY_PATH=/root/sqlanywhere16/lib64:/root/sqlanywhere16/bin64/jre170/lib/amd64/client:/root/sqlanywhere16/bin64/jre170/lib/amd64/server:/root/sqlanywhere16/bin64/jre170/lib/amd64:/root/sqlanywhere16/bin64/jre170/lib/amd64/native_threads:
[1] LS_COLORS=rs=0:di=01;34:ln=01;36:mh=00:pi=40;33:so=01;35:do=01;35:bd=40;33;01:cd=40;33;01:or=40;31;01:mi=00:su=37;41:sg=30;43:ca=30;41:tw=30;42:ow=34;42:st=37;44:ex=01;32:*.tar=01;31:*.tgz=01;31:*.arc=01;31:*.arj=01;31:*.taz=01;31:*.lha=01;31:*.lz4=01;31:*.lzh=01;31:*.lzma=01;31:*.tlz=01;31:*.txz=01;31:*.tzo=01;31:*.t7z=01;31:*.zip=01;31:*.z=01;31:*.Z=01;31:*.dz=01;31:*.gz=01;31:*.lrz=01;31:*.lz=01;31:*.lzo=01;31:*.xz=01;31:*.zst=01;31:*.tzst=01;31:*.bz2=01;31:*.bz=01;31:*.tbz=01;31:*.tbz2=01;31:*.tz=01;31:*.deb=01;31:*.rpm=01;31:*.jar=01;31:*.war=01;31:*.ear=01;31:*.sar=01;31:*.rar=01;31:*.alz=01;31:*.ace=01;31:*.zoo=01;31:*.cpio=01;31:*.7z=01;31:*.rz=01;31:*.cab=01;31:*.wim=01;31:*.swm=01;31:*.dwm=01;31:*.esd=01;31:*.jpg=01;35:*.jpeg=01;35:*.mjpg=01;35:*.mjpeg=01;35:*.gif=01;35:*.bmp=01;35:*.pbm=01;35:*.pgm=01;35:*.ppm=01;35:*.tga=01;35:*.xbm=01;35:*.xpm=01;35:*.tif=01;35:*.tiff=01;35:*.png=01;35:*.svg=01;35:*.svgz=01;35:*.mng=01;35:*.pcx=01;35:*.mov=01;35:*.mpg=01;35:*.mpeg=01;35:*.m2v=01;35:*.mkv=01;35:*.webm=01;35:*.ogm=01;35:*.mp4=01;35:*.m4v=01;35:*.mp4v=01;35:*.vob=01;35:*.qt=01;35:*.nuv=01;35:*.wmv=01;35:*.asf=01;35:*.rm=01;35:*.rmvb=01;35:*.flc=01;35:*.avi=01;35:*.fli=01;35:*.flv=01;35:*.gl=01;35:*.dl=01;35:*.xcf=01;35:*.xwd=01;35:*.yuv=01;35:*.cgm=01;35:*.emf=01;35:*.ogv=01;35:*.ogx=01;35:*.aac=00;36:*.au=00;36:*.flac=00;36:*.m4a=00;36:*.mid=00;36:*.midi=00;36:*.mka=00;36:*.mp3=00;36:*.mpc=00;36:*.ogg=00;36:*.ra=00;36:*.wav=00;36:*.oga=00;36:*.opus=00;36:*.spx=00;36:*.xspf=00;36:
[2] SSH_CONNECTION=192.168.0.10 53832 192.168.0.12 22
[3] LESSCLOSE=/usr/bin/lesspipe %s %s
[4] LANG=C.UTF-8
[5] OLDPWD=/root/sqlanywhere16/bin64
[6] JAVA_HOME=/root/sqlanywhere16/bin64/jre170
[7] XDG_SESSION_ID=6
[8] USER=root
[9] PWD=/root/sqlanywhere16
[10] HOME=/root
[11] SSH_CLIENT=192.168.0.10 53832 22
[12] XDG_DATA_DIRS=/usr/local/share:/usr/share:/var/lib/snapd/desktop
[13] SQLANY16=/root/sqlanywhere16
[14] SQLANYSAMP16=/root/sqlanywhere16/samples
[15] SSH_TTY=/dev/pts/2
[16] MAIL=/var/mail/root
[17] TERM=xterm-256color
[18] SHELL=/bin/bash
[19] SHLVL=1
[20] LOGNAME=root
[21] DBUS_SESSION_BUS_ADDRESS=unix:path=/run/user/0/bus
[22] XDG_RUNTIME_DIR=/run/user/0
[23] PATH=/root/sqlanywhere16/bin64/jre170/bin/:/root/sqlanywhere16/bin64:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin
[24] LESSOPEN=| /usr/bin/lesspipe %s
[25] _=/root/sqlanywhere16/bin64/dbsrv16

SQL Anywhere Network Server Version 16.0.0.2043
Developer edition, not licensed for deployment.

Copyright (c) 2014 SAP AG or an SAP affiliate company.
All rights reserved.
Use of this software is governed by the Sybase License Agreement.
Refer to http://www.sybase.com/softwarelicenses.

Connection limit (licensed seats): 3
Processors detected: 1 (containing 4 logical processors)
Maximum number of processors the server will use: 1 physical processor(s), 2 core(s)
This server is licensed to:
    Developer Edition
    Restricted Use
Running Linux 5.0.0-23-generic #24~18.04.1-Ubuntu SMP Mon Jul 29 16:12:28 UTC 2019 on X86_64
Server built for X86_64 processor architecture
Direct IO disabled for file '/root/sqlanywhere16/demo.db' because the file system on which it resides does not support it
15824K of memory used for caching
Minimum cache size: 15824K, maximum cache size: 14696416K
Using a maximum page size of 4096 bytes
Multiprogramming level: minimum:4, current:20, maximum:80
Automatic tuning of multiprogramming level is enabled
Starting database "demo" (/root/sqlanywhere16/demo.db) at Fri Aug 01 2025 22:13
Direct IO disabled for file '/root/sqlanywhere16/demo.db' because the file system on which it resides does not support it
Transaction log: demo.log
Starting checkpoint of "demo" (demo.db) at Fri Aug 01 2025 22:13
Finished checkpoint of "demo" (demo.db) at Fri Aug 01 2025 22:13
Database "demo" (demo.db) started at Fri Aug 01 2025 22:13
Database server started at Fri Aug 01 2025 22:13
Trying to start SharedMemory link ...
    SharedMemory link started successfully
Trying to start TCPIP link ...
Starting on port 2638
    TCPIP link started successfully
Now accepting requests
Press 'q' to shut down the database server
