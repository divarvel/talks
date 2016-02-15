# Bonnes pratiques de déploiement PHP en 2015


Lorsque j'ai commencé à déployer du PHP, aux alentours de 2002, la mise en
place de cache d'opcode, de reverse proxy pour assets statiques et de
déploiement atomiques était encore rare et peu documentée.

Le monde a évolué, PHP a beaucoup évolué et c'est l'occasion de faire le point
sur les bonnes pratiques de déploiement PHP (en particulier sur une
architecture cloud):

- déploiements reproductibles et automatisables
- déploiement immutables
- séparation code / données
- cache opcode
- séparation serveur HTTP / VM PHP
- gestion des sessions
- gestion des assets

Le but de la présentation est de présenter (et de justifier, en les
contextualisant) ces bonnes pratiques.

## Done

PHP Tour Luxembourg
