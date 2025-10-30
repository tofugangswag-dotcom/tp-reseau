# TP 6

---

## Objectifs du TP
- Faire communiquer deux machines virtuelles sur le même réseau interne.  
- Passer d'une configuration IP statique à une attribution par DHCP.  
- Installer/configurer un serveur DHCP sur une VM.  
- Observer et expliquer le fonctionnement d'ARP (résolution IP ↔ MAC).  
- Savoir extraire et interpréter les preuves (logs, captures, tableaux) pour le rapport.

---


## Exercice 1 

**But** : Mettre des IP statiques sur les deux VM dans le même sous-réseau.  

```bash
# Créer une configuration DHCP via netplan

sudo nano /etc/netplan/01-netcfg.yaml
```

![ezr](https://hackmd.io/_uploads/r1wxnIbkbg.png)
```bash
# appliquer

sudo netplan apply
```

```bash
# je test l'ip avec un ping

ping 192.168.56.99

```
![rezzer](https://hackmd.io/_uploads/HkidhUWkZe.png)
