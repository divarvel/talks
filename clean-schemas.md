# Tips and tricks for clean relational db schemas

## Short

It can be usual for software developers to let the ORM take care of the
database schema. In many cases it's a bad idea as it makes the data stored in
your database brittle and hard to use confidently. I'll show a few tricks
which will help you cleanly store and query data by using your database engine
to its full power.

## Commentary

In some cases, using an ORM brings more problems than solutions. I'll explore
these cases (they are more common than you think) and how to use the freedom
given by having complete control over your schema and your queries:

- indexes
- semantic data types
- query composition
- window functions

I'll show how to still be efficient when going this path (with Jooq / Slick /
Anorm)

## Short FR

Il est courant pour les développeurs de laisser l'ORM décider du schéma de la
base de données. Dans beaucoup de cas c'est une très mauvaise idée, car cela
rend la donnée stockée en base fragile et dure à exploiter en confiance sans
l'ORM. Je montrerai quelques astuces qui aident à stocker et interroger
simplement et proprement de la donnée, en utilisant le moteur de DB comme il
mérite d'être utilisé.

## Commentary FR

Dans certains cas, l'utilisation d'un ORM apporte plus de problèmes que de
solutions. Je passerai en revue certains de ces cas (ils sont plus courants
que l'on ne l'imagine), et je montrerai comment bien employer la liberté
gagnée grâce au contrôle complet sur le schéma et les requètes.

 - index
 - types de données sémantiques
 - composition de requêtes
 - window functions

Bien sûr, je montrerai comment rester efficace au niveau du code avec jooq,
anorm et slick.


## Talk history

It started as a quickie done privately about nice patterns with postgresql (using uuids as primary keys, using expressive types provided by postgresql).
I've enriched it afterwards with more information on how to query a database from applications.
Basically it boils down to:
 - acknowledge the untyped boundary between the application code and the db
 - be very explicit about joins
 - keep your data model flat and close to the db tables.

I've presented it at MixIT, and talk informally about it with flatMap speakers, which also came to the same conclusions than me about how to talk with an ORM.

## Done

BDX.io (2014)
Human Talks (2014)
Devoxx PL (2015)
Tech2Day (2015)
