
## méthode 1 : 

Consultez la commande **arp-scan** - vous devrez probablement l'installer par exemple:

```
sudo apt-get install arp-scan
```

[http://manpages.ubuntu.com/manpages/hardy/man1/arp-scan.1.html](http://manpages.ubuntu.com/manpages/hardy/man1/arp-scan.1.html)

Et pour donner plus de détails :

```
sudo arp-scan --interface=eth0 --localnet
```

Quand eth0 est votre appareil. Vous pouvez trouver votre appareil avec :

```
ifconfig
```


## méthode 2 :


Utilisez nmap. exemple: nmap -sn 10.10.10.0/24 Le cache arp ne vous dira que ceux que vous avez essayé de contacter récemment.