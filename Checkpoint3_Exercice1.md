# Exercice 1 : Manipulations pratiques sur VM Windows (temps estimé : 1h30)
Pour cet exercice tu as besoin de la VM SRVWIN01.

## Partie 1 : Gestion des utilisateurs  
L'utilisateur Kelly Rhameur a quitté l'entreprise.
Elle est remplacée par Lionel Lemarchand

**Q.1.1.1 Créer l'utilisateur Lionel Lemarchand avec les même attribut de société que Kelly Rhameur.**  
<br>
Création nouvel utilisateur
<P ALIGN="center"><IMG src="\Ressources\Q1.1.1_01.png" width=500></P>  

Création mot de passe avec l'option de modification de mot de passe par l'utilisateur lors de la première connexion.
<P ALIGN="center"><IMG src="\Ressources\Q1.1.1_02.png" width=500></P>  

Récapitulatif de la création.
<P ALIGN="center"><IMG src="\Ressources\Q1.1.1_03.png" width=500></P>  

**Q.1.1.2 Créer une OU DeactivatedUsers et déplace le compte désactivé de Kelly Rhameur dedans.**  
<br>
Création de l'OU **DeactivatedUsers**
<P ALIGN="center"><IMG src="\Ressources\Q1.1.2_01.png" width=500></P>  

Déplacement de l'utilisateur **Kelly Rhameur** dans l'OU **DeactivatedUsers**
<P ALIGN="center"><IMG src="\Ressources\Q1.1.2_02.png" width=500></P>  

Confirmation du déplacement.
<P ALIGN="center"><IMG src="\Ressources\Q1.1.2_03.png" width=500></P>  

**Q.1.1.3 Modifier le groupe de l'OU dans laquelle était Kelly Rhameur en conséquence.**  
<br>

Suppression de l'utilisateur **Kelly Rhameur** du groupe **GrpUsersDirectionDesRessourcesHumaines**
<P ALIGN="center"><IMG src="\Ressources\Q1.1.3_01.png" width=500></P>  
Terminer en cliquant sur _Apply_ et _Ok_

Confirmation de la suppression.
<P ALIGN="center"><IMG src="\Ressources\Q1.1.3_01.png" width=500></P>  

**Q.1.1.4 Créer le dossier Individuel du nouvel utilisateur et archive celui de Kelly Rhameur en le suffixant par -ARCHIVE.**  

## Partie 2 : Restriction utilisateurs  
**Q.1.2.1 Faire en sorte que l'utilisateur Gabriel Ghul ne puisse se connecter que du lundi au vendredi, de 7h à 17h.**  

Restriction de connexion pour l'utilisateur **Gabriel Ghul**  
<P ALIGN="center"><IMG src="\Ressources\Q1.2.1_01.png" width=500></P>  

**Q.1.2.2 De même, bloquer sa connexion au seul ordinateur CLIENT01.**  

Restriction de connexion uniquement à la machine **CLIENT01**
<P ALIGN="center"><IMG src="\Ressources\Q1.2.2_01.png" width=500></P>  

**Q.1.2.3 Mettre en place une stratégie de mot de passe pour durcir les comptes des utilisateurs de l'OU LabUsers.**  
<P ALIGN="center"><IMG src="\Ressources\Q1.2.3_01.png" width=500></P>  
<P ALIGN="center"><IMG src="\Ressources\Q1.2.3_02.png" width=500></P>  
<P ALIGN="center"><IMG src="\Ressources\Q1.2.3_03.png" width=500></P>  

## Partie 3 : Lecteurs réseaux  
**Q.1.3.1 Créer une GPO Drive-Mount qui monte les lecteurs E: et F: sur les clients.**  
