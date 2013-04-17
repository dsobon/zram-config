zram-config
===========

Compress swap into ram, effectively doubling ram.

This version has been ported from upstart to sysv init

install
=======
```
$ sudo cp zram-config /etc/init.d/
$ sudo update-rc.d zram-config defaults
$ sudo /etc/init.d/zram-config start
$ free
             total       used       free     shared    buffers     cached
Mem:       6129216    5312200     817016          0      16272    4170752
-/+ buffers/cache:    1125176    5004040
Swap:      3064592          0    3064592
```

requirements
============
* linux kernel 2.6.37 (minimum)
