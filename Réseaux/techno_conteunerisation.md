---
layout: default
title: Comparaison technologies conteneurisation
parent: Réseaux
---

# La conteneurisation et ses technologies

## Qu'est-ce que la conteneurisation ?

C'est le rassemblement entre du code logiciel et l'ensemble des fichiers, des bibliothèques nécessaires pour son bon développement dans une infrastructure. Un exemple simple est lorsque vous avez l'intention d'exécuter une application sur votre ordinateur,
Vous devez avoir une version compatible avec la version de votre système d'exploitation de votre ordinateur.

Grâce à la conteneurisation le problème ne se présente plus étant donné que créer un contenur avec votre application déployée. 
Ce conteneur n'aura donc pas de conflits de comptabilité, car les conteneurs s'exécute sur tous les types d'appareils et système d'exploitation.

## D'où vient la conteneurisation ? 

La conteneurisation est une technologie récente dans le monde de l'informatique, car ses débuts datent de 2001.
Tout commmence avec le projet LinuxVServer, ce projet permettait de faire tourner plusieurs environnements d'exploitation de manière simultanées, mais surtout que chacun des environnement était isolé des autres sur un unique système d'exploitation hôte.
Cette base a permis de créer les multiples technologies en lien avec les conteneurs que l'on connaît aujourd'hui tel que Docker.

En 2008, Docker va se baser LXC en rajoutant une partie de gestion, d'outils et de méthodologie. Durant l'année 2013, Docker est passé open source c'est là que le succès à fait de cette technologie un incourtournable dans le domaine.

C'est alors qu'en 2015, Kubernetes complète les évolutions précédentes en rajoutant une couche d'orchestration qui offre une facilité au niveau de la gestion des conteneurs au travers des clouds publiques.

## Quelles sont les avantages de la conteneurisation ? 

* <b>Portabilité : </b>
La conteneurisation est utilisée par les développeurs de logiciels pour déployer des applications dans divers environnements, sans nécessité une réécriture du code.
 Cela leur permet de créer une seule version d'une application et de la déployer sur différents systèmes d'exploitation. 

* <b>Tolérance aux pannes : </b>
Les développeurs de logiciel utilisent un ensemble de conteneurs pour exécuter des microservices sur le cloud. Étant donné que les conteneurs fonctionnent de manière indépendante, si l'un d'entre eux ne s'exécute pas correctement il n'affectera pas par les autres conteneurs.


* <b>Agilité : </b>
Les applications en conteneurs fonctionnent au sein d'environnements de calcul isolés. Ces environnements offrent aux développeurs la possibilité de résoudre les problèmes et d'apporter des modifications au code sans perturber le système d'exploitation, le matériel ou d'autres services

*<b>Capacité de mise à l’échelle :</b>
Les conteneurs sont des composants logiciels légers qui permettent un démarrage rapide des applications par rapport aux machines virtuelles.
Ils facilitent l'ajout de multiples applications dans différents codétenteurs sur une seule machine.


## Quelles solutions existent à l'heure actuelle ?

* <b>Docker : </b>  
Une plateforme de conteneurisation en accès libre intègre le code source d'une application avec le système d'exploitation existant, ainsi que ses bibliothèques et dépendances. Cette plateforme permet au code de s'exécuter sans problème dans divers environnements informatiques.

* <b>CRI-O : </b>  
C'est une interface d'exécution de conteneurs (CRI) destinée à Kubernetes, une plateforme de gestion de groupes de conteneurs. 
Cette interface assure la compatibilité avec les runtimes de l'OCI. Son rôle principal est de substituer Docker dans l'écosystème de Kubernetes.

* <b>rkt : </b>  
C'est un moteur de conteneurs axé sur les applications, est utilisé pour créer des applications clouds modernes. 
Il repose sur CoreOS et intègre les améliorations de sécurité observées dans les versions précédentes de Docker. Rocket s'intègre bien aux technologies nécessaires et peut être un composant clé d'un système basé sur Docker.

* <b>Kubernetes :</b>  
Kubernetes représente une plateforme ouverte et adaptable qui gère les charges de travail et les services en conteneurs de manière portable.
Elle encourage l'utilisation de configurations déclaratives et l'automatisation des processus. Cette solution s'inscrit dans un écosystème étendu et dynamique.

* <b>LXC : </b>  
Un conteneur fonctionne avec un système d'exploitation unique en son genre, permettant ainsi à une application de s'exécuter de manière virtuelle sur différents systèmes Linux. Ceci est réalisé en utilisant un seul noyau Linux qui agit comme l'environnement d'exploitation principal.


## Comparaison de trois technologies : 

* <b>Docker vs LXC : </b>  
    - Docker supporte la récupération de données, LXC ne le supporte pas
    - LXC est facile d'utilisation et est polyvalent pour la virtualisation
    - Docker ne dépend pas d'un OS, LXC est seulement sur Linux
    - D'un point de vue temps de déploiement Docker est plus efficace

* <b>LXC vs rkt : </b>
    - Les deux fonctionnent sur le système d'exploitation Linux
    - rkt est idéal pour le déploiement rapide des cloud publique
    - LXC a un manque d'intégration de Kubernetess


* <b>rkt vs Docker :</b>
    - rkt n'a pas de démon comparé à Docker 
    - rkt peut s'exécuter plusieurs applications dans un conteneur contrairement à Docker
    - Docker est compatible avec plusieurs systèmes d'exploitation


## Conclusion 

En conclusion, la conteneurisation regroupe le code logiciel et ses dépendances dans des conteneurs isolés, assurant ainsi la portabilité, la tolérance aux pannes et l'agilité. Les technologies clés incluent Docker, CRI-O, rkt et Kubernetes. Docker offre une récupération de données et est compatible avec plusieurs systèmes d'exploitation, tandis que LXC se démarque par sa simplicité.  

rkt convient au déploiement rapide et sécurisé dans le cloud.
La conteneurisation a transformé la façon de développer et de gérer les applications.

## Bibliographie

* [1] https://www.redhat.com/fr/topics/cloud-native-apps/what-is-containerization, consulté le 28/08/2023

* [2] https://aws.amazon.com/fr/what-is/containerization/#:~:text=La%20conteneurisation%20est%20un%20processus,sur%20n'importe%20quelle%20infrastructure.,  consulté le 28/08/2023

* [3] https://www.simform.com/blog/containerization-technology/#:~:text=Expert%20Insight%3A%20For%20example%2C%20by,run%20on%20Windows%20during%20development., consulté le 28/08/2023

* [4] https://www.selceon.com/glossary/conteneurisation-cloud-computing/, consulté le 28/08/2023

* [5] https://kubernetes.io/fr/docs/concepts/overview/what-is-kubernetes/, consulté le 28/08/2023

* [6] https://blog.iron.io/docker-containers-the-pros-and-cons-of-docker/, consulté le 28/08/2023

* [7] https://earthly.dev/blog/lxc-vs-docker/#:~:text=LXC%20provides%20a%20set%20of,application%20in%20an%20isolated%20environment., consulté le 28/08/2023

* [8] https://www.geeksforgeeks.org/difference-between-lxc-and-docker-containers/, consulté le 28/08/2023

* [9] https://stackshare.io/stackups/lxc-vs-rkt, consulté le 28/08/2023

* [10] https://github.com/rkt/rkt, consulté le 28/08/2023

* [11] https://cloudnativenow.com/topics/cloudnativedevelopment/5-container-alternatives-to-docker/, consulté le 28/08/2023

* [12] https://www.educba.com/rkt-vs-docker/, consulté le 28/08/2023