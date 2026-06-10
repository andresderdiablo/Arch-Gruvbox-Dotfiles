Después del archivo, privilegiar en Terminal con: ```sudo chattr +i /etc/resolv.conf```

```
# Quad9 - IPv4 - Principal
nameserver 9.9.9.9

# Quad9 - IPv4 - Secondary
nameserver 149.112.112.112

# Quad9 - IPv6 - Alternative
nameserver 2620:fe::fe
nameserver 2620:fe::9
```