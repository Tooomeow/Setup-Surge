# Setup-Surge
Set up Surge 4 (iOS) by node list

[General]
loglevel = notify
dns-server = dns
skip-proxy = domain
ipv6 = true
http-listen = 0.0.0.0:port
socks5-listen = 0.0.0.0:port
internet-test-url = website
proxy-test-url = website
test-timeout = 1
//#Others#

[Proxy]
Direct = direct
//#(copy from node list)#

[Proxy Group]
AUTO = url-test, #(fill the every proxy name)# , url = website
Group = select, AUTO, #(fill the every proxy name)#, Direct

[Rule]
Final, Group
