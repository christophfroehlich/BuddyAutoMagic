# BuddyAutoMagic
An attempt to make the Buddy/Mentoring/Tutor programslightly more innovative

## INTRODUCTION
Say we want to pair up two groups of people, international students and the local students, with respect to language skills, study level, interests and etc.  We set up an "affinity" score to estimate the affinity of a given pair, a high score indicates that the two persons will like each other.

==============

## License
This is free software, free as in freedom. Feel free to edit it, reuse, redistribute in any way you want. I ask you however to please contribute back to the project if you find it useful.

## Thanks to
Author: **Ólafur Páll Geirsson**

Thanks:
- **Pétur Einarsson** for constant feedback
- **Bjarki Ágúst Guðmundsson** for network flow implementation,
- **Trausti Sæmundsson** for facebook replace regex

## Requirements
Soweit ich das bisher verstanden habe benötigt das System:
- Zwei Formulare mit dazugehörigen Tabellen in die die Daten eingetragen werden.
- Das "große" Spreadsheet mit dem Programmcode von Ólafur das die Berechnungen vornimmt und Einstellungen erlaubt.
- see MailText/readme.txt for Email-integration

## Installation
TODO:

##  Functional principle
We set up a complete [bipartite graph](https://en.wikipedia.org/wiki/Bipartite_graph) with local students on one side and the international students on the other.
We assign the affinity scores as costs to the edges. Our goal:
>   find a perfect matching that maximizes total affinity scores
Matching wird anhand von einem Affinitätswert gemacht wo Leute mit vielen Ähnlichkeiten in eine Gruppe gegeben werden. Dabei hat jeder Buddy mit jedem Incoming ein eigenes Affinity Rating.

## Logger
TODO: how does it work?


## WARNING
The following code does not necessarily follow best coding practices. It was
written to test if pairing students this way could actually work out
