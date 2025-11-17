# notes
Trick for getting wireshark data from other computer in host computer

'ssh root@192.168.12.12 sudo -S tcpdump -i any -U -s0 -w - 'not port 22' | wireshark -k -i -'

![alt text](Fig/remove.png)


Eurecom DNS:
'
  ue_dns:
    primary_ipv4: "172.21.3.100"
    primary_ipv6: "2001:4860:4860::8888"
    secondary_ipv4: "8.8.8.8"
    secondary_ipv6: "2001:4860:4860::8888"
'

#Low latency

https://rigtorp.se/low-latency-guide/

git://git.kernel.org/pub/scm/linux/kernel/git/frederic/dynticks-testing.git

#Isolcpus

$ e "line start when booting"
isolcpus
rcu_nocbs = 4-7
nohz_full = 4-7
rcu_nocb_poll
