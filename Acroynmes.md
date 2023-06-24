
Failles :

LFI : Local File Inclusion -> plusieurs méthodes : ; file_get_contents, include, require, include_once ou require_once doit être enable
info : écrire dans la barre d'url si l'input field ne fonctionne pas
- ../../../../etc/passwd
- ../../../../etc/passwd%00 ou ../../../../etc/passwd0x00
- /répertoire_actuel/../../../../etc/passwd
- ....//....//....//....//etc/passwd

RFI : Remote File Inclusion -> juste mettre l'URL; fonction allow_url_fopen de php enable nécessaire

IDOR : Insecure Direct Object Reference -> ?id=1337

SSRF : Server-Side Request Forgery -> faille qui permet de faire faire une requête http au serveur web, permetterait à priori de récupérer des identifiants ou des trucs du genre

XXS : Cross Site Scripting
- Reflected 
- Stored
- DOM Based
- Blind

Bonus XSS : 
Polyglot : ``jaVasCript:/*-/*`/*\`/*'/*"/**/(/* */onerror=alert('THM') )//%0D%0A%0d%0a//</stYle/</titLe/</teXtarEa/</scRipt/--!>\x3csVg/<sVg/oNloAd=alert('THM')//>\x3e``

Command Injections/Remote Code Execution (RCE) : 
rce vulnerable functions in php :
- exec
- passthru
- system
cheat sheet for payloads : https://github.com/payloadbox/command-injection-payload-list

SQLi : Structured Query Language Injection -> sert à dump, changer ou altérer les données dans les bases de données SQL

**Relational Vs Non-Relational Databases:**  
A relational database, stores information in tables and often the tables have shared information between them, they use columns to specify and define the data being stored and rows to actually store the data. The tables will often contain a column that has a unique ID (primary key) which will then be used in other tables to reference it and cause a relationship between the tables, hence the name **relational** database.  

  

Non-relational databases sometimes called NoSQL on the other hand is any sort of database that doesn't use tables, columns and rows to store the data, a specific database layout doesn't need to be constructed so each row of data can contain different information which can give more flexibility over a relational database.  Some popular databases of this type are MongoDB, Cassandra and ElasticSearch.






DBMS : Database Management System -> peut être Relational ou Non-Relational

Objets Physiques : 

NIC : Network Interface Card
