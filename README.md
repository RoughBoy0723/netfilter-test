# netfilter-test

인풋과 아웃풋을 넷 필터에 넣는다.
sudo iptables -F
sudo iptables -A OUTPUT -j NFQUEUE --queue-num 0
sudo iptables -A INPUT -j NFQUEUE --queue-num 0
