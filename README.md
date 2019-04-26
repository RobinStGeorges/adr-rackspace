# adr-rackspace



VERSION 1 : D�but / systeme de fichiers stoqu�s su chaques machines
======

* Contexte, la probl�matiques, les cas d�utilisation

-un contexte

Les logs sont stoqu�s sur chaques serveurs dans des fichiers textes et acc�d�s � la main par les ing�nieurs

-la probl�matiques

Apr�s un certain nombre de cerveur, le travail devient fastidieux et consomme beaucoup de temps	

-cas d�utilisation

Un utilisateur n'a pas pu envoyer de mail et contact le service client. Ce dernier contact les ing�nieurs, qui se connectent en ssh sur les serveurs afin de recuperer les informations.
	
* Sc�narios d�attribut de qualit� mis en avant

Il s'agit d'un systeme basic simple � mettre en place.

* Vues de structures architecturales pertinentes au regard des attributs choisis

![](./illustrationV1.PNG)

VERSION 2 : Syst�me MySql bas� sur des bases de donn�es relationnel
======

* Contexte, la probl�matiques, les cas d�utilisation 

-un contexte

Mise en place d'une solution MySql ou les logs sont int�gr� � une base de donn�es relationnel, utilisable par le support technique sans l'aide des ing�nieurs
Un Cron s'occupe de l'appel du script de rotation des logs.

-la probl�matiques

Les requetes sont (tr�s) lentes � cause d'un bloquage au niveau des commandes "insert", plus tard am�lior� grace � un systeme de "bulk loading".


-cas d�utilisation

Un utilisateur n'a pas pu envoyer de mail et contact le service client.
	
* Sc�narios d�attribut de qualit� mis en avant

Simplicit�

* Vues de structures architecturales pertinentes au regard des attributs choisis

![](./v2.png)

VERSION 3 : Solution Hadoop
======

* un contexte, la probl�matiques, les cas d�utilisation 

-un contexte

Utilisation d'HADOOP, afin de repartir les taches sur les serveurs dynamiquement. Permet d'eeffectuer des requetes rapidement efficacement et avec des stats.

-la probl�matiques

aucun a part les probl�mes humains.

-cas d�utilisation



* Sc�narios d�attribut de qualit� mis en avant

performance, stabilit�

* Vues de structures architecturales pertinentes au regard des attributs choisis

![](./v3.png)