# Profilesys [![License](https://img.shields.io/:license-mit-yellow.svg)](https://opensource.org/licenses/MIT)

Profilesys is a program that analyzes a systems CPU resources, identifying the NUMA slots and what peripherals belong to what NUMA position.

```
$ ./profilesys 
```

Gives the following output:
```
CPU information
=====================================
Architecture:          x86_64
CPU op-mode(s):        32-bit, 64-bit
Byte Order:            Little Endian
CPU(s):                56
On-line CPU(s) list:   0-55
Thread(s) per core:    2
CPU family:            6
Model name:            Intel(R) Xeon(R) CPU E5-2697 v3 @ 2.60GHz
CPU MHz:               1209.507
CPU max MHz:           3600.0000
CPU min MHz:           1200.0000
Virtualization:        VT-x
L2 cache:              256K
NUMA node0 CPU(s):     0,2,4,6,8,10,12,14,16,18,20,22,24,26,28,30,32,34,36,38,40,42,44,46,48,50,52,54
NUMA node1 CPU(s):     1,3,5,7,9,11,13,15,17,19,21,23,25,27,29,31,33,35,37,39,41,43,45,47,49,51,53,55

Network Card Slot Information
PCI        IntName    PhysSlot   Numa  Driver    
===============================================
01_00_0    eno1       na         0     tg3       
01_00_1    eno2       na         0     tg3       
02_00_0    eno3       na         0     tg3       
02_00_1    eno4       na         0     tg3       
82_00_1    enp130s0f1 na         1     ixgbe     
82_00_0    rename6    na         1     ixgbe     
```
