# Exercice 2 : Manipulations pratiques sur VM Linux (temps estimé : 2h30)
Pour cet exercice tu as besoin de la VM SRVLX01.

## Partie 1 : Gestion des utilisateurs
#### Q.2.1.1 Sur le serveur, créer un compte pour ton usage personnel.

Ajout d'un compte utilisateur avec la commande `adduser`
<P ALIGN="center"><IMG src="\Ressources\Q2.1.1_01.png" width=500></P>  

##### Q.2.1.2 Quelles préconisations proposes-tu concernant ce compte ?

## Partie 2 : Configuration de SSH
Un serveur SSH est lancé sur le port par défaut.
Il est possible de s'y connecter avec n'importe quel compte, y compris le compte root.

#### Q.2.2.1 Désactiver complètement l'accès à distance de l'utilisateur root.

Création d'un fichier backup avant modification du fichier `ssh_config`
<P ALIGN="center"><IMG src="\Ressources\Q2.2.1_01.png" width=500></P>  

Refuser la permition de connexion en tant que Root
<P ALIGN="center"><IMG src="\Ressources\Q2.2.1_02.png" width=500></P>  

#### Q.2.2.2 Autoriser l'accès à distance à ton compte personnel uniquement.

#### Q.2.2.3 Mettre en place une authentification par clé valide et désactiver l'authentification par mot de passe
<P ALIGN="center"><IMG src="\Ressources\Q2.2.3_01.png" width=500></P>  

## Partie 3 : Analyse du stockage
#### Q.2.3.1 Quels sont les systèmes de fichiers actuellement montés ?

#### Q.2.3.2 Quel type de système de stockage ils utilisent ?

Les types de système de stockage utilisés sont RAID1 et LVM
<P ALIGN="center"><IMG src="\Ressources\Q2.3.2_01.png" width=500></P>  

#### Q.2.3.3 Ajouter un nouveau disque de 8,00 Gio au serveur et réparer le volume RAID
<P ALIGN="center"><IMG src="\Ressources\Q2.3.3_01.png" width=500></P>  

#### Q.2.3.4 Ajouter un nouveau volume logique LVM de 2 Gio qui servira à héberger des sauvegardes. Ce volume doit être monté automatiquement à chaque démarrage dans l'emplacement par défaut : /var/lib/bareos/storage.

Utilisation de la commande `lsblk` pour vérifier les disques.
Pour créer la partition LVM sur notre disque, il faut saisire la commande suivant :
```bash
fdisk /dev/sdb
```
<P ALIGN="center"><IMG src="\Ressources\Q2.3.4_01.png" width=500></P>  

#### Q.2.3.5 Combien d'espace disponible reste-t-il dans le groupe de volume ?

## Partie 4 : Sauvegardes
Le logiciel bareos est installé sur le serveur.
Les composants bareos-dir, bareos-sd et bareos-fd sont installés avec une configuration par défaut.

#### Q.2.4.1 Expliquer succinctement les rôles respectifs des 3 composants bareos installés sur la VM.
