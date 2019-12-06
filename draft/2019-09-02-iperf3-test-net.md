---

title: iperf3 测试带宽
date: 2019-09-02
link:

---

上个月刚刚捡垃圾搞来一台网件 R6300V2 ，俗称电磁炉。拿来上手第一时间就刷上了梅林固件，巴拉巴拉一梭子装上 opkg ，接下来就测试一下网速怎样。

```bash
 u0_a21@localhost  ~  iperf3 -c 192.168.0.104 -b 1000m -i 3 -t 120
Connecting to host 192.168.0.104, port 5201
[  5] local 192.168.0.115 port 39340 connected to 192.168.0.104 port 5201
[ ID] Interval           Transfer     Bitrate         Retr  Cwnd
[  5]   0.00-3.00   sec  27.5 MBytes  77.0 Mbits/sec    0    368 KBytes
[  5]   3.00-6.00   sec  34.5 MBytes  96.5 Mbits/sec    0    368 KBytes
[  5]   6.00-9.00   sec  34.5 MBytes  96.5 Mbits/sec    0    368 KBytes
[  5]   9.00-12.00  sec  36.0 MBytes   101 Mbits/sec    0    368 KBytes
[  5]  12.00-15.00  sec  34.6 MBytes  96.8 Mbits/sec    0    368 KBytes
[  5]  15.00-18.00  sec  34.4 MBytes  96.1 Mbits/sec    0    368 KBytes
[  5]  18.00-21.00  sec  35.4 MBytes  98.9 Mbits/sec    0    368 KBytes
[  5]  21.00-24.00  sec  35.9 MBytes   100 Mbits/sec    0    368 KBytes
[  5]  24.00-27.00  sec  35.0 MBytes  97.9 Mbits/sec    0    368 KBytes
[  5]  27.00-30.00  sec  35.4 MBytes  98.9 Mbits/sec    0    368 KBytes
[  5]  30.00-33.00  sec  36.2 MBytes   101 Mbits/sec    0    368 KBytes
[  5]  33.00-36.00  sec  35.5 MBytes  99.3 Mbits/sec    0    368 KBytes
[  5]  36.00-39.00  sec  34.0 MBytes  95.1 Mbits/sec    0    368 KBytes
[  5]  39.00-42.00  sec  36.1 MBytes   101 Mbits/sec    0    368 KBytes
[  5]  42.00-45.00  sec  33.8 MBytes  94.4 Mbits/sec    0    368 KBytes
[  5]  45.00-48.00  sec  33.9 MBytes  94.8 Mbits/sec    0    368 KBytes
[  5]  48.00-51.00  sec  35.4 MBytes  98.9 Mbits/sec    0    368 KBytes
[  5]  51.00-54.00  sec  34.9 MBytes  97.4 Mbits/sec    0    368 KBytes
[  5]  54.00-57.00  sec  35.1 MBytes  98.3 Mbits/sec    0    368 KBytes
[  5]  57.00-60.00  sec  35.1 MBytes  98.2 Mbits/sec    0    368 KBytes
[  5]  60.00-63.00  sec  34.6 MBytes  96.8 Mbits/sec    0    368 KBytes
[  5]  63.00-66.00  sec  34.4 MBytes  96.1 Mbits/sec    0    368 KBytes
[  5]  66.00-69.00  sec  34.6 MBytes  96.8 Mbits/sec    0    368 KBytes
[  5]  69.00-72.00  sec  32.4 MBytes  90.5 Mbits/sec    0    368 KBytes
[  5]  72.00-75.00  sec  33.9 MBytes  94.7 Mbits/sec    0    368 KBytes
[  5]  75.00-78.00  sec  35.0 MBytes  97.8 Mbits/sec    0    368 KBytes
[  5]  78.00-81.00  sec  33.1 MBytes  92.6 Mbits/sec    0    368 KBytes
[  5]  81.00-84.00  sec  32.9 MBytes  91.9 Mbits/sec    0    368 KBytes
[  5]  84.00-87.00  sec  31.6 MBytes  88.3 Mbits/sec    0    368 KBytes
[  5]  87.00-90.00  sec  33.2 MBytes  93.1 Mbits/sec    0    368 KBytes
[  5]  90.00-93.00  sec  32.1 MBytes  89.8 Mbits/sec    0    368 KBytes
[  5]  93.00-96.00  sec  32.8 MBytes  91.6 Mbits/sec    0    368 KBytes
[  5]  96.00-99.00  sec  32.2 MBytes  90.2 Mbits/sec    0    368 KBytes
[  5]  99.00-102.00 sec  34.0 MBytes  95.1 Mbits/sec    0    368 KBytes
[  5] 102.00-105.00 sec  36.1 MBytes   101 Mbits/sec    0    368 KBytes
[  5] 105.00-108.00 sec  34.0 MBytes  95.1 Mbits/sec    0    368 KBytes
[  5] 108.00-111.00 sec  35.2 MBytes  98.6 Mbits/sec    0    368 KBytes
[  5] 111.00-114.00 sec  33.1 MBytes  92.6 Mbits/sec    0    368 KBytes
[  5] 114.00-117.00 sec  35.0 MBytes  97.9 Mbits/sec    0    368 KBytes
[  5] 117.00-120.00 sec  34.8 MBytes  97.2 Mbits/sec    0    368 KBytes
- - - - - - - - - - - - - - - - - - - - - - - - -
[ ID] Interval           Transfer     Bitrate         Retr
[  5]   0.00-120.00 sec  1.34 GBytes  95.6 Mbits/sec    0             sender
[  5]   0.00-120.08 sec  1.34 GBytes  95.6 Mbits/sec                  receiver

iperf Done.
```