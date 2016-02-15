Cet atelier permet de créer une application de chat :
 
 - notification websockets
 - multiple rooms
 - archives
 - bots,
 - webhooks

Tout sera  basé sur RabbitMQ (implémentation AMQP) et sur Akka Stream en
scala. Grâce à RabbitMQ, tout sera scalable (load balancing HTTP et
websocket). Avec Akka Stream, la déclaration des flux de données permettra de
brancher simplement de nouvelles features.

Tout sera déployé en live sur Clever Cloud pour ne pas avoir à gérer des
installations de services locaux. En apprendre plus pas à pas sur ces
nouvelles architectures dans un contexte sécurisant et clair, afin de repartir
avec une vraie expérience sur l’ensemble de ces briques technologiques.

Hands-on très didactique, ciblé sur l'acquisition de compétences concrètes et
précises : faire une API HTTP et websocket qui sait monter en charge avec du
load balancing.

In this hands-on lab, we'll create a chat application :

 - websockets notifications
 - multi rooms
 - archive
 - bots
 - webhooks

Everything will be base on RabbitMQ (AMPQ implementation) and on Akka Streams
in scala. Thanks to RabbitMQ, it will be able to scale out (HTTP and WS load
balancing). With akka streams, the data flow implementation will allow us to
easily add new features.

Everything will be deployed live on clever cloud in order to use remote
services and reduce the setup pains. Step-by-step learning on this new
architecture in a clear an safe context. Attendees will gain real experience
on all these technologies.

We'll show how to create an API that can easily scale out, with code coming
from real project.
