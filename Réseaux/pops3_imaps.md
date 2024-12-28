
---
layout: default
title: POP3S et IMAPS
parent: Réseaux
---

# POPS3 et IMAPS

## D'où proviennent les protocoles POP et IMAP ?

Mark Crispin fut à l'origine de la conception du protocole IMAP en 1986. Après de multiple version, c'est la version 4rev1 encore en vigueur aujourd'hui, qui fut proposée par un groupe de travail de l'IETF en 1996 et mise à jour en 2003. 

Le protocole POP a été mis au point en 1984 par Tim Berners-Lee. Il a également jouer un rôle dans le structuration du World Wide Web. C'est après ce projet qui développa le protocole POP3.

## Qu'est-ce que POP3S ?

Le POP3 (Protocole de Poste version 3) est un protocole de réception de courrier électronique unidirectionnel.
Il permet de télécharger des copies de messages depuis un serveur de messagerie vers un appareil local.
Une fois le téléchargement effectué, le protocole supprime les messages originaux de la boîte de réception du serveur.
Cependant, de nombreux fournisseurs autorisent désormais la conservation des copies originales, ce qui permet aux utilisateurs de consulter le même contenu depuis différentes plateformes.

POP3S est la version sécurisée du protocole, via le port 995.

## Qu-est-ce que IMAPS ?

L'IMAP (Internet Message Access Protocol) est un protocole de réception de courrier électronique.
Les messages sont stockés sur le serveur après avoir été récupérés, ce qui permet d'y accéder depuis différentes plateformes.
Ce protocole assure également une synchronisation entre le client de messagerie et le serveur, facilitant ainsi la communication dans les deux sens.

Comme pour POP, IMAPS est la version sécurisée de ce protocole via le port 993.

## Comment ça marche lorsqu'on envoie un mail et qu'on le réceptionne dans la boîte mail ? 

Un courrier électronique passe par au moins deux serveurs SMTP majeurs appartenant à l'expéditeur et au destinataire.

Initialement, le protocole SMTP établit une connexion entre votre client et le serveur de messagerie de votre fournisseur.
Il examine l'en-tête du courriel pour obtenir des informations qu'il a besoin sur l'expéditeur et le destinataire.

Une fois la destination obtenue, le serveur s'occupe de récupérer l'emplacement du domaine associé à l'adresse. 
Cette information est trouvable dans le système de noms de domaine.

Par exemple, pour un message destiné à utilisateuremail@gmail.com, le serveur localise gmail.com et transfère le message vers cet ordinateur spécifique.

Ensuite, le serveur SMTP du destinataire achemine le message vers la boîte aux lettres du serveur jusqu'à ce que l'utilisateur se connecte à son compte de messagerie.
À ce moment-là, POP3 ou IMAP transfère le nouveau message au client de messagerie du destinataire pour qu'il puisse le visualiser.

## Quelle est la différence POP et IMAP ?

D'un côté POP télécharge les messages sur le serveur et ensuite il les stocke de manière locale sur le poste de travail.

De l'autre côté IMAP s'occupe de faire une synchronisation entre le serveur et le poste de travail de l'utilisateur.

D'une manière générale IMAP est souvent plus intéréssant que son concurrent : 
- étant donné que les messages sont sauvgardés sur le serveur, les mails ne sont jamais perdu 

- IMAP sera capable de récupérer l'organisation de votre boîte de messagerie partout 

- La synchronisation permanente donne une gestion exemplaire des messages.

## Exemple de communication POP3

telnet www.example.com 110
Cette commande ouvre une connexion POP3 à l'www.example.com hôte.

S: + OK <22593.1129980067@example.com>
C: USER foo
S: + OK
C: PASS pluto
S: + OK
C: LISTE
S: + OK
1817
2124
.
C: RETR 1
S: + OK
Return-Path: 
Delivered-To: pippo@example.org
Date: 22 octobre 2005 13:24:54 +0200
De: Mario Rossi 
Objet: xxxx
Content-Type: text / plain; charset = ISO-8859-1
texte du message
.
C: 1 DELE
S: + OK
C: QUIT
S: + OK 

## Conclusion 

En conclusion, les protocoles POP3 et IMAP sont deux protocoles utilisés pour la réception de courrier électronique.
POP3 télécharge les messages du serveur vers le client et les stocke localement, cela peut entraîner une perte de messages si le client n'est pas sauvegardé correctement.
En revanche, IMAP maintient les messages sur le serveur, permettant un accès cohérent depuis plusieurs appareils, ainsi qu'une gestion et une organisation centralisées.
IMAP offre également une synchronisation bidirectionnelle, garantissant que les modifications sont reflétées sur tous les appareils.
 Dans l'ensemble, IMAP tend à offrir une meilleure expérience en termes de gestion des emails modernes.

## Bibliographie

* [1] https://blog.lws-hosting.com/conseils-marketing/comment-fonctionne-un-mail-pop3-smtp-imap#:~:text=Le%20proc%C3%A9d%C3%A9%20est%20simple%2C%20quand,seront%20t%C3%A9l%C3%A9charg%C3%A9s%20sur%20votre%20ordinateur., consulté le 28/08/2023

* [2] https://www.hostinger.fr/tutoriels/mail-pop3-smtp-imap#:~:text=Le%20POP3%20est%20un%20protocole,les%20stocke%20sur%20le%20serveur.

* [3] https://support.google.com/a/answer/12103?hl=fr#:~:text=IMAP%20%3A%20le%20protocole%20IMAP%20permet,un%20t%C3%A9l%C3%A9phone%2C%20par%20exemple)., consulté le 28/08/2023

* [4] https://www.hostinger.fr/tutoriels/mail-pop3-smtp-imap#Qu%E2%80%99est-ce_que_POP3, consulté le 28/08/2023

* [5] https://fr.wikipedia.org/wiki/Post_Office_Protocol, consulté le 28/08/2023

* [6] https://support.microsoft.com/fr-fr/office/que-sont-les-protocoles-pop-et-imap-ca2c5799-49f9-4079-aefe-ddca85d5b1c9#:~:text=IMAP%20vous%20permet%20d'acc%C3%A9der,partir%20du%20service%20de%20messagerie., consulté le 28/08/2023

* [7] https://fr.wikipedia.org/wiki/Post_Office_Protocol, consulté le 28/08/2023

* [8] https://fr.wikipedia.org/wiki/Internet_Message_Access_Protocol consulté le 28/08/2023

* [9] https://boowiki.info/art/protocoles-internet/post-office-protocol.html, consulté le 28/08/2023

* [10] https://trucoteca.com/fr/Qui-est-l%27inventeur-du-protocole-de-communication-pop3-%3F/, consulté le 28/08/2023