---
layout: default
title: IPV4 et IPV6
parent: Réseaux
---

# IPV4 et IPV6

## D'où vient le protcole l'IP ? 

"Une adresse IP (Internet Protocol) est un numéro d'identification unique attribué de façon permanente ou provisoire à chaque périphérique faisant partie d'un même réseau informatique utilisant l'Internet Protocol." Source [3]

Son histoire débute dans les 70, avec la DARPA (l’agence Defense Advanced Research Projects Agency aux États-Unis)?.
Cette agence définir simplement le protocole TCP/IP qui n'était qu'un simple protocole parmi tant d'autres. 
C'est dans un second temps qu'il fut utilisé pour l'ARPAnet comme protocole standard.  

À l'heure actuelle, c'est une norme globale dans le domaine des communications Internet.



## Qu'est-ce que l'IPV4 ?

Le protocole IPV4 constitue la norme pour le format d'adresse, permettant aux appareils de se connecter et de communiquer sur Internet.
Les adresses IPv4 sont des valeurs numériques encodées sur 32 bits. Elle est divisée en quatres nombres, chacun compris entre 0 et 255, et sont séparées par des points.

Vous avez probablement déjà entendu parler de l'idée d'une adresse IP, et il est fort probable que vous ayez déjà repéré la vôtre.
Cette information est généralement présentée sous cette forme : 192.168.1.1. 
Le protocole IPv4 permet la création de plus de 4 milliards d'adresses uniques, ce qui a été extrêmement utile pendant plusieurs décennies.

## Qu'est-ce que l'IPV6 ?

Le protocole IPV6, est la version suivante de IPV4.
Il a même rôle qui d'être un valeur unique permettant d'identifier un appareil dans un réseau.
En effet, tandis que l'architecture du protocole IPv4 autorisait la création de 4 milliards d'adresses, l'IPv6 offre une capacité de 340 sextillions d'adresses.
L'IPv6 est basé sur une notation hexadécimale à 128 bits, et son format habituel est le suivant :

2001:0ab8:85a2:0000:0000:8a3e:0370:7334

Son modèle de conception a été simplifié pour permettre une meilleure adaptation à l'environnement actuel.

## Qu'est-ce que l'IPV6 à de plus que l'IPV4 ?


* Amélioration du routage sans fragmentation des paquets : IPv6 améliore l'efficacité du routage en évitant la fragmentation des paquets, ce qui contribue à une meilleure transmission des données.

* Intégration de la Qualité de service (QoS) pour la reconnaissance des paquets prioritaires : Dans IPv6, la qualité de service est intégrée pour identifier et donner la priorité aux paquets importants, assurant ainsi des performances optimales.

* Élimination du NAT pour étendre l'espace d'adressage de 32 à 128 bits : IPv6 résout les limitations d'adressage d'IPv4 en élargissant l'espace d'adressage à 128 bits, éliminant ainsi la nécessité d'utiliser des techniques de traduction d'adresses réseau (NAT).

* Sécurité de couche réseau intégrée (IPsec) : IPv6 intègre nativement des mécanismes de sécurité, renforçant la protection des communications en ligne.

* Configuration automatique des adresses sans état pour faciliter l'administration réseau : IPv6 propose des méthodes de configuration automatique des adresses, simplifiant la gestion et l'administration des réseaux.

* Amélioration de la structure d'en-tête et réduction des coûts de traitement : L'en-tête d'IPv6 a été optimisé pour être plus efficace, ce qui diminue les exigences de traitement lors du routage des paquets.


## Quelle est l'avenir de l'IPV6 ?

L'IPV6 est arrivé suite à la pénurie d'adresse IPV4, il faut donc un candidat suivant pour reprendre la suite du protocole IP. Certains problèmes se posent : 

- Le matériel est trop ancien pour l'IPV6
- Les responsables d'entreprise ne voient pas utile de migrer vers l'IPV6
- La formation sur l'IPV6 est encore au minimum  (école, université)

Malgré ces problématiques, le monde va devoir s'adapter à cette nouveauté, car l'IPV4 ne possède plus d'adresses.

## Conclusion 

En conclusion,IPv6 apporte des améliorations telles qu'un routage plus efficace, la Qualité de Service intégrée, et une sécurité renforcée.
Cependant, son adoption est freinée par l'obsolescence matérielle, la réticence des entreprises et le manque de formation.
Malgré cela, la transition vers IPv6 est essentielle pour garantir la connectivité à long terme.

## Bibliographie


* [1] https://www.techno-science.net/definition/10887.html, consulté le 28/08/2023

* [2] https://www.ionos.fr/digitalguide/serveur/know-how/quels-sont-les-avantages-de-ipv6, consulté le 28/08/2023

* [3] https://fr.wikipedia.org/wiki/Adresse_IP#:~:text=RFC%20791%20%E2%80%94%20Internet%20Protocol%2C%20septembre%201981%20(IP)., consulté le 28/08/2023

* [4] https://kinsta.com/fr/blog/ipv4-vs-ipv6/#:~:text=La%20diff%C3%A9rence%20la%20plus%20%C3%A9vidente,moins%20dans%20un%20futur%20proche)., consulté le 28/08/2023

* [5] https://blog.ataxya.net/ipv6-lavenir-dinternet/, consulté le 28/08/2023

* [6] https://www.avg.com/fr/signal/what-is-tcp-ip#:~:text=Cr%C3%A9%C3%A9%20%C3%A0%20l'origine%20dans,pr%C3%A9d%C3%A9cesseur%20de%20l'Internet%20moderne., consulté le 28/08/2023

* [7] https://www.juniper.net/fr/fr/research-topics/what-is-ipv4-vs-ipv6.html, consulté le 28/08/2023