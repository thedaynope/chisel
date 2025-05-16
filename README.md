# linux server tab 1
$ chisel server -p 51080 -v
# linux server tab 2
$ iperf -s -u -p 4444

# macbook tab 1
$ chisel client -v <server-ip>:51080 3333:4444/udp
# macbook tab 2
$ iperf -c localhost -u -p 3333 -b 100m
