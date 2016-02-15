# Acknowledging boundaries: how to bring back consistency to your microservice architecture.

# Les bornes des limites : comment maintenir de la cohérence dans votre architecture microservices

## Long

Most of us are moving away from big, monolithic architectures. The rise of
commodity hardware and the increasing need for flexibility in business
constraints make it the best choice. By doing so, we gain lots of good things:
scalability, smaller code bases, asynchronous deployments, and the ability to
pick the right tech stack for every module.

But by splitting our architecture, we push complexity to the boundaries
between systems. Consistency which was ensured by an atomic codebase and type
systems is now impossible to assert. Many communication layers try to hide the
boundaries to make communication between modules transparent. This is where
things can go wrong. Acknowledging the boundaries and the loss of information
which is inherent to them make it easier to tame the complexity introduced by
a microservice architecture.

In this presentation I'll show how taking boundaries into account reduces risk
of inconsistent data.  I'll show how to encode messages between bricks to
explicitely state, for each module, what structure is needed, and what should
be able to evolve without impacting the module. Implicit serialization may be
simpler at the beginning, but explicit serialization helps a lot, especially
when dealing with asynchronous deployments and heterogeneous code bases. This
is one place where the type system can help a lot and bring back confidence.

At Clever Cloud, we have an heterogeneous architecture: some modules are in
JavaEE, some in scala, some in Ruby, some in javascript, some in Perl.
Maintaining integrity throughout the platform is tough, and proper
architecture as well as data modelling is of prime importance.

I'll show examples in javascript and scala, as well as draw comparisons to my
experience in web development, where there is extensive information about what
happens when developpers try to blur boundaries between server-side and
client-side.

This session is suitable for people with all levels. Code examples will be
simple and well explained: there are just there to serve as concrete examples,
not to demonstrate advanced features of the languages.

## Short + commentary

### Short

Most of us are moving away from big, monolithic architectures.
By doing so, we gain lots of good things: scalability, smaller code bases,
asynchronous deployments, and the ability to pick the right
tech stack for every module.

But by splitting our architecture, we push complexity to the boundaries
between systems. Consistency which was ensured by an atomic codebase and type
systems is now impossible to assert.

In this presentation I'll show how taking boundaries into account reduces risk
of inconsistent data.  I'll show how to encode messages between bricks to
explicitely state, for each module, what structure is needed, and what should
be able to evolve without impacting the module. Implicit serialization may be
simpler at the beginning, but explicit serialization helps a lot.

I'll show examples in javascript and scala, as well as draw comparisons to my
experience in web development, where there is extensive information about what
happens when developpers try to blur boundaries between server-side and
client-side.

### Short fr

La tendance est au délaissement des architectures monolithiques au profit de
micro-services bien découpés. Ainsi nous facilitons le passage à l'échelle,
réduisons la taille de chaque projet et pouvons utiliser la pile techno
adaptée à chaque module.

Cependant, en séparant ces briques, nous repoussons la complexité à la limite
entre chaque module. La cohérence fournie par une base de code atomique et son
système de types est perdue.

Dans cette session, je montrerai comment tenir compte explicitement des
frontières entre modules permet de réduire le risque de données incohérentes.
Je montrerai comment encoder les messages inter-modules, en déclarant
explicitement pour chaque brique, la structure nécessaire et ce qui doit
pouvoir évoluer sans impacter le module. La *serialisation* implicite a beau
etre plus simple au début, l'explicite aide beaucoup.

Je donnerai des exemples en scala et javascript, tout en tirant des
comparaisons avec mon expérience en développement web, où on a une expérience
fournie de ce qui se passe quand les développeurs essayent d'ignorer les
frontières entre coté serveur et coté client.

### Commentary


When splitting an application in several modules, we often try to have
transparent communication between the modules. This may seem simpler but it
pushes business logic into the void between modules (see "complexity is
outside the code" by Dan North & Jessica Kerr at Codemesh 2014). My point is
to encode knowns and unknowns at every module boundary. Inside of every module
it allows to get back the confidence given by a monolithic yet modular code.

### Commentary fr

Quand on sépare une application en plusieurs modules, il est courant d'essayer
d'avoir une communication transparente entre les briques (RMI, Serializable,
…). Cela peut sembler plus simple, mais cela conduit à repousser la logique
métier dans l'espace immatériel entre les briques (cf la keynote "complexity is
outside the code" de Dan North & Jessica Kerr à Codemesh 2014). Le but du talk
est de montrer comment encoder les ce que l'on sait et ce que l'on peut
ignorer à chaque frontière de module. Ainsi, au sein de chaque module on peut
récupérer la cohérence et la confiance que l'on peut avoir dans un code
monolithique mais modulaire.

