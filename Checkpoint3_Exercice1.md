# Exercice 1 : Manipulations pratiques sur VM Windows (temps estimé : 1h30)
Pour cet exercice tu as besoin de la VM SRVWIN01.

## Partie 1 : Gestion des utilisateurs  
L'utilisateur Kelly Rhameur a quitté l'entreprise.
Elle est remplacée par Lionel Lemarchand

**Q.1.1.1 Créer l'utilisateur Lionel Lemarchand avec les même attribut de société que Kelly Rhameur.**  

Création nouvel utilisateur  
![CatureQ.1.1.1](./Ressources/Q1.1.1_01.png)
 
Création mot de passe avec l'option de modification de mot de passe par l'utilisateur lors de la première connexion.
![CatureQ.1.1.1](./Ressources/Q1.1.1_02.png)

Récapitulatif de la création.  
![CatureQ.1.1.1](./Ressources/Q1.1.1_03.png)
 
**Q.1.1.2 Créer une OU DeactivatedUsers et déplace le compte désactivé de Kelly Rhameur dedans.**  

Création de l'OU **DeactivatedUsers**   
![CatureQ.1.1.2](./Ressources/Q1.1.2_01.png)  

Déplacement de l'utilisateur **Kelly Rhameur** dans l'OU **DeactivatedUsers**  
![CatureQ.1.1.2](./Ressources/Q1.1.2_02.png)

Confirmation du déplacement.   
![CatureQ.1.1.2](./Ressources/Q1.1.2_03.png)  

**Q.1.1.3 Modifier le groupe de l'OU dans laquelle était Kelly Rhameur en conséquence.**  

Suppression de l'utilisateur **Kelly Rhameur** du groupe **GrpUsersDirectionDesRessourcesHumaines**  

![CatureQ.1.1.3](./Ressources/Q1.1.3_01.png)
Terminer en cliquant sur _Apply_ et _Ok_

Confirmation de la suppression.  
![CatureQ.1.1.3](./Ressources/Q1.1.3_02.png)  

**Q.1.1.4 Créer le dossier Individuel du nouvel utilisateur et archive celui de Kelly Rhameur en le suffixant par -ARCHIVE.**  

## Partie 2 : Restriction utilisateurs  
**Q.1.2.1 Faire en sorte que l'utilisateur Gabriel Ghul ne puisse se connecter que du lundi au vendredi, de 7h à 17h.**  

Restriction de connexion pour l'utilisateur **Gabriel Ghul**  
![CatureQ.1.2.1](./Ressources/Q1.2.1_01.png)

**Q.1.2.2 De même, bloquer sa connexion au seul ordinateur CLIENT01.**  

Restriction de connexion uniquement à la machine **CLIENT01**  
![CatureQ.1.2.2](./Ressources/Q1.2.2_01.png)

**Q.1.2.3 Mettre en place une stratégie de mot de passe pour durcir les comptes des utilisateurs de l'OU LabUsers.**  
![CatureQ.1.2.3](./Ressources/Q1.2.3_01.png)
![CatureQ.1.2.3](./Ressources/Q1.2.3_02.png)
![CatureQ.1.2.3](./Ressources/Q1.2.3_03.png)

## Partie 3 : Lecteurs réseaux  
**Q.1.3.1 Créer une GPO Drive-Mount qui monte les lecteurs E: et F: sur les clients.**  
