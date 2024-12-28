---
layout: default
title: Firewall
parent: Sécurité
---

# Firewall

## Qu'est-ce qu'un Firewall ?

Un pare-feu est un dispositif de sécurité réseau. Son rôle est de surveiller le trafic que ce soit entrant ou sortant, avec ses informations il prend la décision d'autoriser ou de bloquer, la partie du trafic concernée. Ces décisions sont dépendantes des règles définies lors de la configuration de ce pare-feu.  

Les pare-feu existent sous deux formes distinctes :
- Matériel 
- Logiciel 

Il peut être comme un service basé sur un logiciel, un second rôle est d'être hébergé sur cloud de manière virtuelle ou encore il peut-être connecté après un routeur afin de sécuriser un serveur.

## Quel est son histoire ?

Les firewalls appelés pare-feu en français, existent depuis la fin des années 80. Leur but premier était de filtrer les paquets lorsqu'il y avait un transfert d'un ordinateur à un autre.À l'heure actuelle ce type de pare-feu existe toujours.

L'année 1993, Monsieur Shwed qui est à l'époque le dirigeant de Check Point à lancé son tout premier Firewall appelé "FireWall-1". Cette première réalisation était équipé de technologie Stateful Inspection.

Des années plus tard, son avancée technologique restera le premier rempart en matière de sécurisation pour les entreprises contre les cyberattaques.

## Quelles sont les types de Firewall qui existent ?
 
* <b>Pare-feu proxy :</b>  
C'est la passerelle entre deux réseaux pour une application spécifique. Il offre également des fonctionnalités de mise en cache de contenu, de mise en cache de la protection. Il procède en bloquant les connexions directes depuis l'extérieur du réseau.
* <b>Pare-feu à inspection(stateful) :</b>  
Ce pare-feu est considéré comme le plus standard actuellement, son fonctionnement est simple : il bloque une partie du trafic en fonction des ports, des protocoles et de l'état du trafic. Les décisions sont définies sur les règles mises en place par l'administrateur.
* <b>Pare-feu de gestion unifiée des risques liés à la sécurité (UTM) :</b>  
Un pare-feu de gestion unifiée des risques de sécurité combine en partie les caractéristiques d'un pare-feu à inspection avec des fonctionnalités de prévention des intrusions et d'antivirus. Généralement il intègre la gestion du cloud.
* <b>Pare-feu de nouvelle génération (NGFW) :</b>  
Les pare-feux de nouvelle génération sont une évolution des pare-feux classiques tel que le pare-feu à inspection. Ces nouveaux dispositifs de sécurité doivent également être capables de :
    - "Un contrôle d'accès basé sur la Threat Intelligence avec inspection « stateful »"
    - "Un système de prévention des intrusions (IPS) intégré"
    - "La reconnaissance et le contrôle des applications pour détecter et bloquer celles qui présentent un risque"
    - "Des voies d'évolution afin d'inclure les futurs flux d'informations"
    - "Des techniques pour faire face à l'évolution des menaces pour la sécurité"
    - "Le filtrage des URL en fonction de la géolocalisation et de la réputation"
    - Source : [5]
* <b>Pare-feu virtuel :</b>  
 Ce type de pare-feu est déployé en tant qu'application logiciel utilisé dans un environnement  virtuel dans un cloud privé (VMWare ESXi : cfr Admin III) ou un cloud public (AWS, Microsoft Azure). Son rôle est de contrôler et protéger que ce soit le trafic physique et virtuel.
* <b>Pare-feu cloud natif :</b>  
 Concernant le pare-feu cloud natif, il est conçu pour les environnements de type cloud. Il offre de nombreux avantages pour la gestionnaire d'administration réseau comme l'agilité et la flexibilité de sa sécurité. 

## Quelles sont ses avantages ?

* <b>Sécurité :</b>  
La sécurité de l'ordinateur ainsi que du réseau, c'est le premier rempart face au danger que peut-être internet.
* <b>Contrôle :</b>  
Un de ses avantages est le contrôle sur la communication avec les informations. Il permet d'éviter que certaines informations personnelles soient transmises sans que vous ne le sachiez. 
Il joue un rôle dans la protection de la vie privée des utilisateurs.
* <b>Perfomance : </b>  
Un pare-feu peut également permettre d'améliorer les performances d'un ordinateur ou du réseau car il bloque le trafic inutile ce qui réduit une partie des informations à traiter.
* <b>Conformité : </b>  
Enfin, un pare-feu peut aider à être en ordre face aux exigences réglementaires et aux normes industrielles. Cet aspect est pour les entreprises et les organisations soumises à des directives spécifiques, visant à sécuriser les informations confidentielles.

## Quelles sont ses inconvénients ?

* <b>Complexité : </b>  
La complexité se présente lors de la configuration pour les utilisateurs peu informés sur les concepts liés au réseau. 
* <b>Coût : </b>  
Dans le cas des entreprises cela peut-être coûteux d'avoir un pare-feu. La maintenance, les mises à jour peuvent entraîner des coûts permanents.
* <b>Performance : </b>  
Parfois les pare-feux peuvent ralentir les perfomances de l'ordinateur.
* <b>Comptabilité :  </b>  
Lorsqu'un pare-feu est mis en place dans un un système, il se peut que certaines applications ne soient pas comptabiles avec celui-ci.

## Conclusion

En Conclusion, un pare-feu représente le point central de la sécurité informatique en tant que dispositif de protection réseau. Il surveille et contrôle le trafic entrant et sortant, contribuant ainsi à empêcher les menaces potentielles tout en offrant des avantages essentiels. Il garantit la sécurité des systèmes et des données, assure un contrôle précis sur les communications, et peut améliorer les performances en filtrant les flux inutiles. 

Cependant, il est important de noter que les pare-feux peuvent présenter des complexités dans leur configuration, des coûts en termes de maintenance et de mises à jour, ainsi que des défis potentiels en matière de performances et de compatibilité avec certaines applications. En fin de compte, malgré ces inconvénients, leur rôle central dans la protection des informations sensibles et la conformité aux réglementations en font un outil indispensable pour les entreprises et les organisations.

## Bibliographie

* [1] https://www.forcepoint.com/fr/cyber-edu/firewall

* [2] https://www.checkpoint.com/fr/cyber-hub/what-is-firewall/#:~:text=Historique%20des%20Firewall,un%20ordinateur%20%C3%A0%20un%20autre., consulté le 28/08/2023

* [3] https://www.cisco.com/c/fr_fr/products/security/firewalls/what-is-a-firewall.html, consulté le 28/08/2023

* [4] https://www.fortinet.com/fr/resources/cyberglossary/hardware-firewalls-better-than-software, consulté le 28/08/2023

* [5] https://www.cisco.com/c/fr_fr/products/security/firewalls/what-is-a-firewall.html#~types-de-pare-feu, consulté le 28/08/2023

* [6] https://aspiringyouths.com/advantages-disadvantages/firewall/?utm_content=cmp-true, consulté le 28/08/2023