# adr-rackspace

How Rackspace Now Uses MapReduce and Hadoop to Query Terabytes of Data


-an early amoeba'ic text file stored on each machine
	Had to be manually searched by engineers 
	Had to log into each systems
	Was replaced by a script 
-a Neandertholic relational database solution that just couldn't compete
	Mysql based solution
	Could not keep with the data flow increase
-a Homo sapien'ic Hadoop based solution that works wisely for them and has virtually 
	unlimited scalability potential

VERSION 1 : Début / systeme de fichiers stoqués su chaques machines
======

  * un contexte, la problématiques, les cas d’utilisation
    *un contexte
	Les logs sont stoqués sur chaques serveurs et accédés à la main par les ingénieurs
    *la problématiques
	Les ingénieurs ont besoin d'avoir les logs des servers afin d'aider à resoudre les problème le plus vite possible	
  * les scénarios d’attribut de qualité mis en avant
  * des vues de structures architecturales pertinentes au regard des attributs choisis


VERSION 2 : Système MySql basé sur des bases de données relationnel
======

  * un contexte, la problématiques, les cas d’utilisation 
	La version précédente prend trop de temps car manuel, besoin d'une solution automatique 
  * les scénarios d’attribut de qualité mis en avant
  * des vues de structures architecturales pertinentes au regard des attributs choisis


VERSION 3 : Solution Hadoop
======

  * un contexte, la problématiques, les cas d’utilisation 
	les requetes et les logs stoqués ralentissent les serveurs
  * les scénarios d’attribut de qualité mis en avant
  * des vues de structures architecturales pertinentes au regard des attributs choisis

