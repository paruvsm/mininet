####  <b>install-requirement-vlan-md</b>

[Need to do first]

1. sudo apt-get install bridge-utils
2. sudo apt-get install vlan
3. sudo modprobe 8021q


<b>1. sudo apt-get install bridge-utils</b>
<pre>
bertopeng17@bertopeng17-ThinkPad-T520:~$ <b>sudo apt-get install bridge-utils</b>
[sudo] password for bertopeng17: 
Reading package lists... Done
Building dependency tree       
Reading state information... Done
The following packages were automatically installed and are no longer required:
  linux-headers-3.19.0-25 linux-headers-3.19.0-25-generic
  linux-image-3.19.0-25-generic linux-image-extra-3.19.0-25-generic
Use 'apt-get autoremove' to remove them.
The following NEW packages will be installed:
  bridge-utils
0 upgraded, 1 newly installed, 0 to remove and 0 not upgraded.
Need to get 29,1 kB of archives.
After this operation, 145 kB of additional disk space will be used.
Get:1 http://id.archive.ubuntu.com/ubuntu/ trusty/main bridge-utils i386 1.5-6ubuntu2 [29,1 kB]
Fetched 29,1 kB in 2s (10,8 kB/s)       
Selecting previously unselected package bridge-utils.
(Reading database ... 297613 files and directories currently installed.)
Preparing to unpack .../bridge-utils_1.5-6ubuntu2_i386.deb ...
Unpacking bridge-utils (1.5-6ubuntu2) ...
Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
Setting up bridge-utils (1.5-6ubuntu2) ...
bertopeng17@bertopeng17-ThinkPad-T520:~$
</pre>

<b>2. sudo apt-get install vlan</b>

<pre>
bertopeng17@bertopeng17-ThinkPad-T520:~$ <b>sudo apt-get install vlan</b>
Reading package lists... Done
Building dependency tree       
Reading state information... Done
The following packages were automatically installed and are no longer required:
  linux-headers-3.19.0-25 linux-headers-3.19.0-25-generic
  linux-image-3.19.0-25-generic linux-image-extra-3.19.0-25-generic
Use 'apt-get autoremove' to remove them.
The following NEW packages will be installed:
  vlan
0 upgraded, 1 newly installed, 0 to remove and 0 not upgraded.
Need to get 30,2 kB of archives.
After this operation, 163 kB of additional disk space will be used.
Get:1 http://id.archive.ubuntu.com/ubuntu/ trusty/main vlan i386 1.9-3ubuntu10 [30,2 kB]
Fetched 30,2 kB in 1s (16,6 kB/s)
Selecting previously unselected package vlan.
(Reading database ... 297639 files and directories currently installed.)
Preparing to unpack .../vlan_1.9-3ubuntu10_i386.deb ...
Unpacking vlan (1.9-3ubuntu10) ...
Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
Setting up vlan (1.9-3ubuntu10) ...
bertopeng17@bertopeng17-ThinkPad-T520:~$ 
</pre>

<b>3. sudo modprobe 8021q</b>

<pre>
bertopeng17@bertopeng17-ThinkPad-T520:~$ sudo modprobe 8021q
bertopeng17@bertopeng17-ThinkPad-T520:~$ 

</pre>
