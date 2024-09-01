# netfilter-test

sudo iptables -F
sudo iptables -A output -j NFQUEUE --queue-num 0
sudo iptables -A input -j NFQUEUE --queue-num 0

iptables를 이용하여 넷 필터에서 패킷을 큐에 담아서 C언어를 사용하여 패킷을 필터링할 수 있다.
