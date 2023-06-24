la table users :
![[Pasted image 20230624133903.png]]



`select * from users;` : retourne toute toute la table users
![[Pasted image 20230624145327.png]]
`select username,password from users;` : retourne les colonnes username et password de la table users
![[Pasted image 20230624145339.png]]
`select * from users LIMIT 1;` : retourne seulement la première row de la table users 
![[Pasted image 20230624145350.png]]
`select * from users LIMIT 1,1;` : retourne toutes les rows sauf la première de la table users
`select * from users LIMIT 2,1;` : retourne toutes les rows sauf les deux premières de la table users

`select * from users where username='admin';` : retourne seulement la row qui contiendrait l'username "admin" dans la table users
![[Pasted image 20230624145402.png]]
`select * from users where username != 'admin';` : retourne toutes les row qui ne contiennent pas l'username "admin"
![[Pasted image 20230624145423.png]]
`select * from users where username='admin' or username='jon';` : retourne les rows qui contiennent les usernames "admin" ou "jon"
![[Pasted image 20230624145434.png]]
`select * from users where username='admin' and password='p4ssword';` : retourne la row qui a comme username "admin" et pour password "p4ssword"
![[Pasted image 20230624145445.png]]
`select * from users where username like 'a%';` : retourne toutes les rows qui ont un username qui commence par "a"; exemple : admin
![[Pasted image 20230624145454.png]]
`select * from users where username like '%n';` : retourne toutes les rows qui ont un username qui se termine par "n"; exemple : jon, admin, martin
![[Pasted image 20230624145513.png]]
`select * from users where username like '%mi%';` : retourne toutes les rows qui ont un username qui contient les caractères "mi"; exemple : admin
![[Pasted image 20230624145531.png]]
`SELECT name,address,city,postcode from customers UNION SELECT company,address,city,postcode from suppliers;` : combine le contenu de deux tables à conditions que leurs colonnes soient les mêmes

exemple :
- la table "customers" :
![[Pasted image 20230624143623.png]]
- la table "suppliers" : 
![[Pasted image 20230624143728.png]]

résultat de l'instruction `SELECT name,address,city,postcode from customers UNION SELECT company,address,city,postcode from suppliers;` : 
![[Pasted image 20230624143833.png]]

`insert into users (username,password) values ('bob','password123');` : sert à insérer une nouvelle row dans la table users qui a pour username "bob" et pour mot de passe "password123"
![[Pasted image 20230624145554.png]]
`update users SET username='root',password='pass123' where username='admin';` : sert à changer la valeur "username" de l'username "admin" en lui assignant comme nouvelle valeur "root" et comme nouvelle password "pass123" dans la table users
![[Pasted image 20230624144224.png]]

`delete from users where username='martin';` : sert à supprimer la row qui contient l'username "martin"  de la table users
![[Pasted image 20230624145056.png]]

`delete from users;` : sert à supprimer toute la table users car il n'y a pas d'instruction WHERE 
![[Pasted image 20230624145618.png]]

`database()` : fonction SQL permettant d'obtenir le nom de la base de donnée 

à faire des notes sur ça plus tard : 


![[Pasted image 20230624151944.png]]
![[Pasted image 20230624152012.png]]

