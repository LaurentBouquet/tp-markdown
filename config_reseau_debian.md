# Configuration réseau de mon serveur Debian

## Introduction

Bienvenue sur la documentation de mon réseau. Ici, vous trouverez toutes les infos nécessaires pour comprendre ma configuration.

## Détails de la configuration

Voici les étapes que j'ai suivies pour configurer mon réseau :

1. Mise à jour du système
2. Installation des outils réseau
3. Configuration de l'interface réseau
4. Test de la connectivité

### Mise à jour du système

Pour commencer, mettez à jour votre système avec la commande suivante :

```sh
sudo apt-get update && sudo apt-get upgrade
```

### Installation des outils réseau

Installez les outils nécessaires :

```sh
sudo apt-get install net-tools
```

### Configuration de l'interface réseau

Voici un exemple de configuration pour `/etc/network/interfaces` :

```sh
auto eth0
iface eth0 inet static
address 172.16.138.10
netmask 255.255.0.0
gateway 172.16.138.250
```

### Test de la connectivité

Testez votre connexion avec `ping` :

```sh
ping -c 4 google.com
```

## Conclusion

Vous devriez maintenant avoir un réseau fonctionnel sur votre serveur Debian. N'hésitez pas à me contacter pour toute question !