# TDD, as in Type-Directed Development

## Short

Test-Driven Development is widely accepted as good practice. But can we do
better? By specifying your program's behaviour with types, you can go a very
long way, with more confidence and with less hassle than with tests.

In this talk, I will show a new vision of types, explore the fundamental
differences between specifying with types and specifying with tests. I'll talk
about how types allow us to prove properties about our program and how
genericity is a tremendously powerful tool for specification. He'll show means
of reasoning based on types and assess specifically what it provides.  Lastly,
I will show how to complement Type-Directed Development with Test-Driven
Development to specify with tests what's left after laying out the types.

## Short fr

Le développement dirigé par les tests (TDD) est largement considéré comme une
bonne pratique. Mais pouvons-nous faire mieux ? En spécifiant le comportement
attendu d'un programme avec des types, on peut aller très loin, avec plus de
confiance et moins de complications qu'avec des tests.

Dans ce talk, je montrerai une autre vision des types, en explorant la
différence fondamentale entre types et tests au niveau des spécifications.
J'aborderai la manière dont les types permettent de prouver des propriétés sur
les programmes et pourquoi les génériques sont l'outil le plus puissant à
votre disposition. Je momnterai des moyens de raisonner basés sur les types et
décrirai ce qu'ils apportent. Enfin, je montrerai comment complémenter le
Type-DD avec le Test-DD pour finir de spécifier avec des tests ce qui n'a pas
pu être spécifié par des types


## Commentary

The idea is to start from a simple case in java, and then go on showing all
the possible error cases hidden in it. The handling of all those cases will
change the code structure, making it brittle, harder to read and understand.
Worst of all, the code structure won't have anything in common with the
problem structure.  By using explicit types, I'll show how previously hidden
error cases will be put in plain light just by observing the types stucture.
The code structure will then be aligned again with the problem structure.
I'll showcase a few simple ways to encode more information in types (Optional,
nonEmptyList, tagged types, newtyping…)

Then I'll show how generics are the most powerful way to encode information
in types, and how it can serve as documentation.

Lastly, I'll show how to combine tests (property-based, then unit tests) with
types.

I gave this presentation as a closing keynote at lambdacon, and as the opening
keynote of Java Day Ukraine. It is well received by both functional
programmers and OO-programmers.

## Done

Scala.io (2014)
CodeMesh.io (2014)
TDD Geecon (2014)
Lambda Con (2015)
Java Day Ukraine (2015)
Softshake (2015)
