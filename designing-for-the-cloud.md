# Designing for the cloud

# Short EN

Migrating a legacy application to the cloud can be challenging. The path to
the 12 factor app is not an easy one to take, but can be incredibly rewarding,
even if you end up not deploying in the cloud.

In this talk I'll show you why cloud-readiness and scalability are just
by-products of good design, and how modern architectures like microservices
can be a very good fit with cloud-friendly architectures.

By the end of the presentation you will be able to:

 - rethink state in your web applications to ease scalability
 - handle files at scale with file storage APIs
 - split your services with message queues
 - handle persistent connections like websocket at scale

# Short FR

Migrer une application legacy vers le cloud, ça n'est pas toujours facile. La
route vers 12factor est semée d'embûche mais est extrêmement rentable, même si
vous n'allez pas jusqu'au déploiement continue dans le cloud

Dans ce talk, je vais montrer pourquoi la "Cloud-Readiness™" et la scalabilité
dérivent directement d'une bonne conception et comment les visions "modernes",
comme par exemples les microservices se marient très bien avec des archis
"cloud-friendly".

À la fin de la présentation, vous aurez vu comment :

 - concevoir la gestion de l'état dans vos applis web pour faciliter la scalabilité
 - gérer du stockage de fichier à l'échelle avec les APIs de stockage de fichier
 - découpler vos services avec les message brokers
 - gérer les connexions persistentes (par exemple les websockets) dans un
   contexte distribué

# Commentary EN


I've helped quite a few customers going from a legacy setup to a cloud
deployement.  This talk is a recap of the advice I usually give, plus a way to
show that these modifications are not constraints but that they are overall
good design.

HTTP is stateless by its very nature, so a stateful HTTP service is the result
of hidden dependencies to state. Moving to a cloud setup forces you to expose
and manage these dependencies, but that's something you should do anyway.

# Commentary FR

J'ai aidé de nombreux clients à passer d'une infra legacy à un déploiement
cloud. Ce talk reprend les conseils et les recommandations que je donne
régulièrement, tout en soulignant que ce ne sont pas des restrictions
arbitraires mais des bons conseils au global.

# History

Internal presentations in several startups (2015 & 2016)
ScaleConf NZ 2016 (Pending)
