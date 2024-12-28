---
layout: default
title: Seveur web et ses technologies
parent: Réseaux
---

# Seveur web et ses technologies

## C'est quoi un serveur web ?

D'un point de vue matériel, un serveur web est un ordinateur où l'on retrouve tous les composants pour construire un site web. Ces composants sont : les pages html, les feuilles de style css, les fichiers javascript. 
Lorsque l'utilisateur va vouloir visiter le site, l'ordinateur qui est connecté à Internet va envoyer l'ensemble de ses composants à celui-ci pour que la page s'affiche chez l'utilisateur.

D'un point de vue logiciel, le rôle du serveur web est s'occuper de la manière dont les utilisateurs ont accès aux fichiers hébergés. La base de celui-ci est un serveur http, c'est en quelques sortes un logiciel comprenant une liste d'URL.

Prenons un cas pratique d'exemple, fait une requête HTTP vers le serveur pour avoir accès au fichier. Le serveur lui répond en lui envoyer le fichier par la même requête HTTP.

Il existe deux types de serveurs web :
 - Statique : Il est basé avec un d'un ordinateur et d'un serveur htttp
 - Dynamique : Composé d'autres composants logiciels tel qu'une base de données.


## C'est quoi Apache ? 

Apache fait partie des serveurs web le plus ancien du marché, sa présence remonte à 1995.
C'est un logiciel open-source et multi-plateforme, selon certains chiffres ce serait le serveur web le plus utilisé du marché actuellement.
Sa popularité lui a permis de conquérir des grands noms de ce monde tel que : Cisco, IBM, eBay, etc.

## C'est quoi Nginx ?

Nginx qui le grand concurrent d'Apache est un également un serveur web open-source, il s'est fait connaître en tant que serveur web mais actuellement il joue plusieurs rôles tels que reverse proxy, cache HTTP ou load balancer. 

- Un reverse proxy :  
 "Pour résumer, un serveur proxy est un intermédiaire de communication sur le réseau qui reçoit les requêtes pour les transmettre ensuite à l’ordinateur cible. 
Dans les réseaux des entreprises, ce système est particulièrement utilisé pour fournir un accès à Internet plus sécurisé et davantage contrôlable pour les utilisateurs.
Un serveur configuré comme proxy représente dans ce cas l’unique connexion au réseau public." Source : [10]

- Une cache HTTP :  
"Un cache correspond à un stockage local de données reçues précédemment ou plus exactement des messages de réponse HTTP reçus précédemment. 
Un système de cache contrôle le stockage, la récupération et la suppression de ces messages." : Source : [11]

- Un loard balancer:  
"Le load balancer est réalisé par un équipement dédié, une appliance physique ou virtuelle. 
Cette appliance identifie en temps réel quel serveur au sein d'un pool répond le mieux à une demande donnée du client, tout en veillant à ce qu'un trafic réseau intense ne surcharge pas trop un seul et même serveur." : Source [12]


## C'est quoi Lighttpd ?

C'est un logiciel serveur web écrit en C, définit comme flexible, rapide et sécurisé. 
Son CPU ayant une plus petite empreinte mémoire que la plupart des serveurs web lui permet d'être plus rapide. Sa première apparition date de 2003.
En Avril 2007, il faisait partie des 5 serveurs web les plus utilisé du marché. 
Malgré la domination d'Apache ainsi que Nginx dans le domaine il reste néanmoins utilisé. 


## Comparaison entre les 3 technologies :

### Tableau comparatif 

|   Nom|   Open source|   Prix|   Avantages | Inconvénients |
|---    |:-:    |:-:    |:-    |:--    |
|   Apache |   Oui   |   Gratuit | Logiciel stable, Mise à jour régulière, facile à configurer, cela s'adapte facilement aux débutants | Problèmes de performances sur les sites web avec un énorme trafic |
|   Nginx   |   Oui  |   Gratuit |    Meilleur evolutivité dans le temps qu'Apache, conçu sur mesure donc de bonnes performances | Nginx ne prend pas en charge .htaccess, pas comme Apache| 
|   Lighttpd   |   Oui   |  Sur demande |   Il est rapide, flexible, il a de bonnes peformances | Cela ne supporte pas les fichiers htaccess ou encore htpasswd pas comme Apache| 

## Conclusion 

En Conclusion, un serveur web est un ordinateur hébergeant les composants d'un site (HTML, CSS, JavaScript). Les serveurs web gèrent l'accès à ces fichiers.
Apache, le plus vieux et stable, est largement utilisé malgré des problèmes de performances pour les sites très fréquentés.  

Nginx, concurrent d'Apache, évolue bien dans le temps, performant pour les connexions multiples, mais ne supporte pas certaines fonctionnalités d'Apache.
Lighttpd, rapide et flexible, performant aussi, mais moins populaire.

## Bibliographie

* [1] https://developer.mozilla.org/fr/docs/Learn/Common_questions/Web_mechanics/What_is_a_web_server, consulté le 28/08/2023

* [2] https://detechter.com/the-battle-of-the-web-servers-apache-vs-nginx-vs-lighttpd-2/, consulté le 28/08/2023

* [3] https://kinsta.com/fr/base-de-connaissances/qu-est-ce-qu-apache/, consulté le 28/08/2023

* [4] https://kinsta.com/fr/base-de-connaissances/qu-est-ce-que-nginx/, consulté le 28/08/2023

* [5] https://fr.wikipedia.org/wiki/Lighttpd, consulté le 28/08/2023

* [6] https://detechter.com/the-battle-of-the-web-servers-apache-vs-nginx-vs-lighttpd-2/, consulté le 28/08/2023

* [7] https://iwf1.com/apache-vs-nginx-vs-lighttpd-comparing-performance-resource-usage-and-features/2, consulté le 28/08/2023

* [8] https://www.hostinger.fr/tutoriels/quest-ce-quapache-serveur-web-apache, consulté le 28/08/2023

* [9] https://www.opportunites-digitales.com/guide-complet-du-serveur-nginx/, consulté le 28/08/2023

* [10] pierre-giraud.com/http-reseau-securite-cours/cache/, consulté le 28/08/2023

* [11] https://www.ionos.fr/digitalguide/serveur/know-how/quest-ce-quun-reverse-proxy-le-serveur-reverse-proxy/, consulté le 28/08/2023

* [12] https://www.lemagit.fr/definition/Load-balancer-repartition-de-charge, consulté le 28/08/2023