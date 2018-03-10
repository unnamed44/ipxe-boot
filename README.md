


include-menu.ipxe  
```
#!ipxe

dhcp
chain --replace --autofree tftp://${next-server}/ipxe-boot/boot.ipxe ||
chain --replace --autofree http://boot.unnamed.info/ipxe-boot/boot.ipxe ||
chain --replace --autofree https://raw.githubusercontent.com/unnamed44/ipxe-boot/master/boot.ipxe
```


