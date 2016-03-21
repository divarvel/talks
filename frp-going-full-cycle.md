# Beyond flux: going full cycle with functional reactive programming.

# Short

React and flux have shown us how to design UI in a modular fashion. One of the
core ideas, is that data should always flow in one direction. With this
concept, it's easier to build applications from independent modules. I'll show
what react core concepts are and how they allow developers to manage
complexity in big applications.

I'll then show how to go one step further with Functional Reactive Programming
and RxJS. After explaining what FRP is (and isn't), I'll show how FRP
principles can unify a lot of different things in flux architectures. Cycle.js
allows us to have a single direction rendering loop by representing both DOM
and user interaction with observables, which come with an extensive API.

FRP has been used for some time in UI frameworks (eg Reactive Cocoa for
MacOS). Now its time has come in the javascript world, thanks to libraries
like RxJS and to the ideas pushed forward by React and Flux.

At the end of the talk, you'll have a basic understanding of how Flux works,
you'll know how RxJS works and how you can use FRP to design your client side
applications.

# Short

React et flux nous ont montré comment concevoir des interfaces utilisateur
modulaires. L'idée principale est que la donnée se déplace toujours dans une
seule direction. Grâce à ce concept, il est simple de créer des applications à
partir de composants indépendants. Je montrerai quels sont les principes
fondamentaux de react et comment ils permettent aux développeurs de gérer
la complexité de grosses applications.

Je montrerai ensuite comment aller plus loin avec la programmation
fonctionnelle réactive (FRP). Je décrirai la FRP puis je montrerai comment la
FRP unifie les concepts présents dans flux.

Cycle.js nous fournit une boucle de rendu unidirectionnelle en représentant le
DOM et les interactions utilisateurs par des observables, briques de base de la
FRP et qui fournissent une API très complète.

La FRP est utilisée depuis un moment pour la création d'UI (par ex. Reactive
Cocoa pour MacOS). Le moment est venu de s'en servir en JS, grâce à des
bibliothèques comme RxJS et à des idées poussées par React et Flux

À la fin du talk vous aurez une compréhension simple de comment marchent Flux,
RxJS et vous saurez comment utiliser la FRP pour concevoir vos applications
client-side.

# Commentary

Flux is very powerful but quite complicated and built on tools that are not
really suited writing to reactive applications. Hence the complexity of flux
and its reputation to be hard to understand by beginners.

The ideas made popular by react and flux (single direction rendering,
immutable data, etc) map very cleanly to FRP building blocks: observables.

Building client side applications with this concepts allows a very declarative
and easy to understand interaction model. Cycle.js may seem too simple to be
useful, but its power really lies in its simplicity.

I've given this talk at NantesJS in French, so I can give it both in French
and in English.


# History

NantesJS (2015)
JsConfIs (2016 - pending)
