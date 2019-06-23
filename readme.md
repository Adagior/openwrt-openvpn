'''
iptables -I FORWARD -o br-lan -j ACCEPT
iptables -I FORWARD -o tun0 -j ACCEPT
iptables -t nat -A POSTROUTING -s 192.168.1.0/24 -j MASQUERADE



openvpn --cd /etc/openvpn --config /etc/openvpn/vegas.ovpn
'''

https://gist.github.com/willwhui/1febd37a3dd79a503cc8544c3bb18ece
http://blog.jqian.net/post/openwrt-openvpn.html
