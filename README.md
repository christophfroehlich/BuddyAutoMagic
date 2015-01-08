# BuddyAutoMagic
An attempt to make the Buddy/Mentoring/Tutor programslightly more innovative

## INTRODUCTION
Say we want to pair up two groups of people, international students and the local students, with respect to language skills, study level, interests and etc.  We set up an "affinity" score to estimate the affinity of a given pair, a high score indicates that the two persons will like each other.

==============

## Copyright
This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.


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
- see [MailText/how2SetupMailText.md](MailText/how2SetupMailText.md) for Email-integration

## Installation
Open up the spreadsheets containing your form responses and look at the url, it will be something like:    https://docs.google.com/spreadsheet/ccc?key=0ApBBsTPBxGcMdHBRbEg0cTdkczFjcWw4d0RxdW53clE&usp=drive_web#gid=6
Extract the key (e.g. "0ApBBsTPBxGcMdHBRbEg0cTdkczFjcWw4d0RxdW53clE" in this case) and insert it in buddyAutoMagic.gs
TODO:

##  Functional principle
We set up a complete [bipartite graph](https://en.wikipedia.org/wiki/Bipartite_graph) with local students on one side and the international students on the other.
We assign the affinity scores as costs to the edges. Our goal:
>   find a perfect matching that maximizes total affinity scores

## Logger
TODO: how does it work?


## WARNING
The following code does not necessarily follow best coding practices. It was
written to test if pairing students this way could actually work out
