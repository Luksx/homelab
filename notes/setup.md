# Nastavení VMware

Rozhodl jsem se simulace provádět v VMware virutalizačním softwaru. I přes to že se jedná o virtualizaci nad windows, alternativní Hyper-V má mnohem slabší podporu pro linuxové systéme než VMware. Takže VMware byl jasná cesta.

Nastavil jsem 3 vmware sítě:

- Lokální síť

- Síť NAT

- Síť host-vm

Taky jsem pro začátek rozjel virtualizační mašiny:

- Debian server

- OPNsense firewall server

- Void linux (client)

Proč zrovna Void linux jako client? Běžím na nich už nějakou dobu a jejich rychlost je nepřekonatelná (obzvlášť do VM).

> Chvíli jsem tedy bojoval s open-vm-tools na voidu, ale nakonec se vše podařilo

### Mapa sítě

OPNsense funguje jako firewall a je zároveň tedy komponent, který rozděluje lokální síť (LAN). Na LAN hostuje DHCP server. 

![net-map.png](pictures/net-map.svg)

Debian server má na DHCP serveru nastavenou statickou IP adresu. Taky je serveru přiřazen hostname *debian.lab.internal*.

