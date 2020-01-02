RESOURCES
---------

STORAGE
-------

Filesystem     1K-blocks      Used Available Use% Mounted on
udev            16457664         0  16457664   0% /dev
tmpfs            3293960       792   3293168   1% /run
/dev/xvda1       8065444   1683624   6365436  21% /
tmpfs           16469788         0  16469788   0% /dev/shm
tmpfs               5120         0      5120   0% /run/lock
tmpfs           16469788         0  16469788   0% /sys/fs/cgroup
/dev/loop0         91264     91264         0 100% /snap/core/7713
/dev/loop1         18432     18432         0 100% /snap/amazon-ssm-agent/1480
/dev/xvdf      314419200 310203460   4215740  99% /data
tmpfs            3293956         0   3293956   0% /run/user/1000


CPU
---

top - 14:59:51 up 35 min,  1 user,  load average: 1.16, 1.09, 0.92
Tasks: 153 total,   1 running,  81 sleeping,   0 stopped,   0 zombie
%Cpu(s): 14.5 us,  0.6 sy,  0.0 ni, 84.5 id,  0.0 wa,  0.0 hi,  0.3 si,  0.2 s
KiB Mem : 32939576 total,   569496 free,  2564328 used, 29805752 buff/cache
KiB Swap:        0 total,        0 free,        0 used. 29910584 avail Mem 

  PID USER      PR  NI    VIRT    RES    SHR S  %CPU %MEM     TIME+ COMMAND   
 8300 ubuntu    20   0 5810888 2.351g 109916 S 138.5  7.5  32:41.76 bitcoind  
    1 root      20   0  225356   9032   6696 S   0.0  0.0   0:03.03 systemd   
    2 root      20   0       0      0      0 S   0.0  0.0   0:00.01 kthreadd  
...


FILES
-----

ls -lR $CHAIN_DATA

-rw------- 1 ubuntu ubuntu        37 Dec 28 14:31 banlist.dat
drwxr-xr-x 6 ubuntu ubuntu        73 Nov 18 09:44 bitcoin-0.19.0.1
-rw-rw-r-- 1 ubuntu ubuntu      1357 Dec 28 14:27 bitcoin.conf
-rw------- 1 ubuntu ubuntu         5 Dec 28 14:31 bitcoind.pid
drwx------ 3 ubuntu ubuntu     94208 Dec 28 20:13 blocks
drwx------ 2 ubuntu ubuntu        74 Dec 28 14:31 chainstate
drwx------ 2 ubuntu ubuntu        50 Dec 28 14:31 database
-rw------- 1 ubuntu ubuntu         0 Dec 28 14:31 db.log
-rw------- 1 ubuntu ubuntu 152828387 Dec 28 21:13 debug.log
drwx------ 3 ubuntu ubuntu        21 Dec 28 14:31 indexes
-rw------- 1 ubuntu ubuntu   1006028 Dec 28 21:01 peers.dat
-rw------- 1 ubuntu ubuntu   1470464 Dec 28 14:31 wallet.dat


DIRECTORIES
-----------

ls -lR                  |wc  15891  142696  974803
ls -lR blocks           |wc   3879   34872  243906
ls -lR chainstate       |wc      6      39     233
ls -lR database         |wc      4      21     147
ls -lR indexes          |wc  11941  107430  728138
ls -lR indexes/txindex/ |wc  11937  107418  728064



./bitcoin-0.19.0.1:
total 4
-rw-r--r-- 1 ubuntu ubuntu 3983 Nov 18 09:44 README.md
drwxr-xr-x 2 ubuntu ubuntu  119 Nov 18 09:44 bin
drwxr-xr-x 2 ubuntu ubuntu   32 Nov 18 09:44 include
drwxr-xr-x 2 ubuntu ubuntu  104 Nov 18 09:44 lib
drwxr-xr-x 3 ubuntu ubuntu   17 Nov 18 09:44 share

./bitcoin-0.19.0.1/bin:
total 74256
-rwxr-xr-x 1 ubuntu ubuntu  3129176 Nov 18 09:44 bitcoin-cli
-rwxr-xr-x 1 ubuntu ubuntu 33559560 Nov 18 09:44 bitcoin-qt
-rwxr-xr-x 1 ubuntu ubuntu  3621720 Nov 18 09:44 bitcoin-tx
-rwxr-xr-x 1 ubuntu ubuntu  6977216 Nov 18 09:44 bitcoin-wallet
-rwxr-xr-x 1 ubuntu ubuntu 11439032 Nov 18 09:44 bitcoind

-rwxr-xr-x 1 ubuntu ubuntu 17298048 Nov 18 09:44 test_bitcoin

./bitcoin-0.19.0.1/include:
total 4
-rw-r--r-- 1 ubuntu ubuntu 3711 Nov 18 09:44 bitcoinconsensus.h

./bitcoin-0.19.0.1/lib:
total 436
lrwxrwxrwx 1 ubuntu ubuntu     28 Nov 18 09:44 libbitcoinconsensus.so -> libbitcoinconsensus.so.0.0.0
lrwxrwxrwx 1 ubuntu ubuntu     28 Nov 18 09:44 libbitcoinconsensus.so.0 -> libbitcoinconsensus.so.0.0.0
-rwxr-xr-x 1 ubuntu ubuntu 444560 Nov 18 09:44 libbitcoinconsensus.so.0.0.0

./bitcoin-0.19.0.1/share:
total 0
drwxr-xr-x 3 ubuntu ubuntu 18 Nov 18 09:44 man

./bitcoin-0.19.0.1/share/man:
total 0
drwxr-xr-x 2 ubuntu ubuntu 109 Nov 18 09:44 man1

./bitcoin-0.19.0.1/share/man/man1:
total 52
-rw-r--r-- 1 ubuntu ubuntu  3676 Nov 18 09:44 bitcoin-cli.1
-rw-r--r-- 1 ubuntu ubuntu 18695 Nov 18 09:44 bitcoin-qt.1
-rw-r--r-- 1 ubuntu ubuntu  3267 Nov 18 09:44 bitcoin-tx.1
-rw-r--r-- 1 ubuntu ubuntu  1972 Nov 18 09:44 bitcoin-wallet.1
-rw-r--r-- 1 ubuntu ubuntu 18245 Nov 18 09:44 bitcoind.1

./blocks:
-rw------- 1 ubuntu ubuntu 134212906 Dec 28 14:34 blk00000.dat
-rw------- 1 ubuntu ubuntu 134206860 Dec 28 14:34 blk00001.dat
...
-rw------- 1 ubuntu ubuntu 133755374 Dec 28 20:13 blk01910.dat
-rw------- 1 ubuntu ubuntu 100663296 Dec 28 21:13 blk01911.dat
drwx------ 2 ubuntu ubuntu        74 Dec 28 14:31 index
-rw------- 1 ubuntu ubuntu  19503073 Dec 28 14:34 rev00000.dat
-rw------- 1 ubuntu ubuntu  17825792 Dec 28 14:34 rev00001.dat
...
-rw------- 1 ubuntu ubuntu  17811056 Dec 28 20:13 rev01910.dat
-rw------- 1 ubuntu ubuntu  13631488 Dec 28 21:13 rev01911.dat
./blocks/index:
total 8
-rw------- 1 ubuntu ubuntu  0 Dec 28 14:31 000003.log
-rw------- 1 ubuntu ubuntu 16 Dec 28 14:31 CURRENT
-rw------- 1 ubuntu ubuntu  0 Dec 28 14:31 LOCK
-rw------- 1 ubuntu ubuntu 50 Dec 28 14:31 MANIFEST-000002

./chainstate:
total 12
-rw------- 1 ubuntu ubuntu 46 Dec 28 14:31 000003.log
-rw------- 1 ubuntu ubuntu 16 Dec 28 14:31 CURRENT
-rw------- 1 ubuntu ubuntu  0 Dec 28 14:31 LOCK
-rw------- 1 ubuntu ubuntu 50 Dec 28 14:31 MANIFEST-000002

./database:
total 1576
-rw------- 1 ubuntu ubuntu 1048576 Dec 28 14:31 log.0000000003
-rw------- 1 ubuntu ubuntu 1048576 Dec 28 14:31 log.0000000004

./indexes:
total 40
drwx------ 2 ubuntu ubuntu 24576 Dec 28 15:00 txindex

./indexes/txindex:
-rw------- 1 ubuntu ubuntu       216 Dec 28 16:58 039235.ldb
-rw------- 1 ubuntu ubuntu   2169581 Dec 28 17:00 041430.ldb
-rw------- 1 ubuntu ubuntu   2173526 Dec 28 17:00 041431.ldb
... 
-rw------- 1 ubuntu ubuntu   2175471 Dec 28 20:03 102736.ldb
-rw------- 1 ubuntu ubuntu   2147547 Dec 28 20:03 102737.ldb
-rw------- 1 ubuntu ubuntu 186605698 Dec 28 20:06 102739.ldb
-rw------- 1 ubuntu ubuntu 100532760 Dec 28 21:13 102740.log
-rw------- 1 ubuntu ubuntu 186580800 Dec 28 20:11 102741.ldb
-rw------- 1 ubuntu ubuntu        16 Dec 28 14:31 CURRENT
-rw------- 1 ubuntu ubuntu         0 Dec 28 14:31 LOCK
-rw------- 1 ubuntu ubuntu  14529673 Dec 28 20:11 MANIFEST-000002

