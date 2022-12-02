# Secure
Les types d'attaques et des exemples
# Exercice de recherche portant sur la sécurité des bases de données 

# Partie 1 : Citez les types d'attaques et les attaques relatifs aux bases de données

|Type d'attaques                     |Attaques      |          
|------------------------------------|--------------|
|Une mauvaise presse de information (confidentialité)  | injection SQL, Abus de privilège excessif, Abus de privilège légitime ,Exploitation des failles des bases de données vulnérables ou mal configurées , Elévation de privilège , Copies non autorisées de données sensibles,Exposition de données de sauvegarde,
|Modifier des données(intégrité) |   Exploitation des failles des bases de données vulnérables ou mal configurées , Faiblesse de l’audit natif  
|Disponibilite                  |    Déni de services      


# Partie 2 : Norme de sécurité des ITSEC
   Les ITSEC définissent la politique de 
sécurité comme l’ensemble des lois règles 
ou pratiques qui régissent la façon dont 
l’information sensible et les autres 
ressources sont gérées, protégées et 
distribuées à l’intérieur d’un système 
d’information.


# Partie 3 : Fichiers dans lesquelles sont stockés les données dans les SGBD tels que MYSQL ,POSTGRESSQL , ORACLE ,MSSQLSERVER 

 ## SQL SERVER

 Au minimum, chaque base de données SQL Server a deux fichiers de système d’exploitation : un fichier de données et un fichier journal. Les fichiers de données contiennent des données et des objets tels que des tables, des index, des procédures stockées et des vues. Les fichiers journaux contiennent les informations nécessaires pour récupérer toutes les transactions de la base de données. Les fichiers de données peuvent être regroupés dans des groupes de fichiers à des fins d'allocation et d'administration

Les fichiers de données se situent généralement dans un répertoire enfant nommé « Data ». Par exemple, spécifiez C:\Program Files\Microsoft SQL Server\MSSQL{nn}.<nom_instance>\ comme chemin racine du répertoire de données des bases de données système durant la mise à niveau quand les fichiers de données se trouvent sous C:\Program Files\Microsoft SQL Server\MSSQL{nn}.<nom_instance>\MSSQL\Data.


  ## MYSQL

Dans Windows 8.1, les bases de données MySQL sont stockées (par défaut) ici: C:\ProgramData\MySQL\MySQL Server 5.6\data 

Le dossier C:\ProgramData est un dossier caché. Vous devez donc le saisir dans l’adresse de l’explorateur Windows pour y accéder. Dans ce dossier de données, les bases de données sont nommées /{database_name_folder}/{database_tables_and_files}. 

Par exemple, 

C:\ProgramData\MySQL\MySQL Server 5.6\data\mydatabase\mytable.frm
C:\ProgramData\MySQL\MySQL Server 5.6\data\mydatabase\mytable.ibd


## ORACLE

Les fichiers de données sont les fichiers occupant la majeure partie de la base de données, leur taille peut osciller entre quelques Mégaoctets et plusieurs gigaoctets. Ceux-ci contiennent en effet toutes les données relatives à la base Oracle dans un format propriétaire. Ainsi pour modifier les informations contenues dans la base de données il est impossible d'intervenir directement sur ces fichiers; la bonne procédure à adopter consiste à modifier le contenu de la base de données par l'intermédiaire d'ordres SQL.

Les fichiers de données contiennent des informations de deux types :

* Le dictionnaire de données et de travail
* Les données des utilisateurs
* La lecture de ces fichiers de données est faite à l'aide des * processus utilisateurs tandis que l'écriture est assuré par le processus DBWR (Database Writer)

## POSTGRESQL
Comme tous les SGBD relationnel, PostGreSQL stocke les données
des tables et des index dans des fichiers organisés sous forme de
pages

Traditionnellement, les fichiers de configuration et les fichiers de données utilisés par une instance du serveur sont stockés ensemble dans le répertoire des données, habituellement référencé en tant que PGDATA (d'après le nom de la variable d'environnement qui peut être utilisé pour le définir). Un emplacement courant pour PGDATA est /var/lib/pgsql/data. Plusieurs groupes, gérés par différentes instances du serveur, peuvent exister sur la même machine.

##PARTIE QUESTION SUR SQL ET CES NORMES
*Norme Actuelle :Publié ISO/IEC 9075-1:2016 (Une norme est révisée tous les 5 ansPublié)
*Une norme est révisée tous les 5 ans
*En cours d’élaboration : ISO/IEC DIS 9075-1

La norme SQL n'est pas distribuée gratuitement. La norme complète peut être achetée auprès de l'ISO.
La norme est découpée selon les parties suivantes3:

*ISO/CEI 9075-1:2011 [archive] Framework

*ISO/CEI 9075-2:2011 [archive] Foundation

*ISO/CEI 9075-3:2008 [archive] Call-Level Interface

*ISO/CEI 9075-4:2011 [archive] Persistent Stored Modules

*ISO/CEI 9075-9:2008 [archive] Management of External Data

*ISO/CEI 9075-10:2008 [archive] Object Language Bindings

*ISO/CEI 9075-11:2011 [archive] Information and Definition Schemas

*ISO/CEI 9075-13:2008 [archive] SQL Routines and Types Using the Java Programming Language

*ISO/CEI 9075-14:2011 [archive] XML-Related Specifications

*La partie la plus importante est la partie 2, qui est aussi la plus longue avec 1470 pages, soit 100 pages de plus que pour SQL:2008. Les parties manquantes sont 
des parties qui ont été retirées pour diverses raisons, lorsqu'un numéro de partie est utilisé il n'est plus réutilisé

