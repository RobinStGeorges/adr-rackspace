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

VERSION 1 : D�but / systeme de fichiers stoqu�s su chaques machines
======

  * un contexte, la probl�matiques, les cas d�utilisation
    *un contexte
	Les logs sont stoqu�s sur chaques serveurs et acc�d�s � la main par les ing�nieurs
    *la probl�matiques
	Les ing�nieurs ont besoin d'avoir les logs des servers afin d'aider � resoudre les probl�me le plus vite possible	
  * les sc�narios d�attribut de qualit� mis en avant
  * des vues de structures architecturales pertinentes au regard des attributs choisis


VERSION 2 : Syst�me MySql bas� sur des bases de donn�es relationnel
======

  * un contexte, la probl�matiques, les cas d�utilisation 
	La version pr�c�dente prend trop de temps car manuel, besoin d'une solution automatique 
  * les sc�narios d�attribut de qualit� mis en avant
  * des vues de structures architecturales pertinentes au regard des attributs choisis


VERSION 3 : Solution Hadoop
======

  * un contexte, la probl�matiques, les cas d�utilisation 
	les requetes et les logs stoqu�s ralentissent les serveurs
  * les sc�narios d�attribut de qualit� mis en avant
  * des vues de structures architecturales pertinentes au regard des attributs choisis

