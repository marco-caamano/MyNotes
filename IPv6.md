# IPv6 notes

## IPv6 Addresses

- IPv6 addresses are 128bit wide.

## IPv6 Unicast Address

Packets are delivered to a single device or interface

### Global Unicast Address (GUA)

- Equivalent to IPv4 public addresses. 
- Routable. 
- Assigned by Internet Registries

Format 2000::/3
Example 2001:db8::1

### Link Local Address

- Automatically configured on each interface
- Not routable beyond local link (subnet / L2 domain)

Format FE80::/10

Example: FE80::1a2b:001


### Unique Local Address (ULA)

- Equivalent to IPv4 private addresses (192.168.x.x, 10.x.x.x, etc)
- Not routable

Format FC00::/7

Example: FD00::1

### Loopback Address

Format



### Add IPv6 IP to interface

```
ip -6 addr add df88::dead:beef:0001/64 dev enp0s3
```
