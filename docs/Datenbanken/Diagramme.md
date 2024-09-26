# Diagramme
## ERD (Entity-Relationship-Diagrams)
Eine ERD Diagram (*ausg*.: **E**ntity **R**elationship **D**iagram; *deu*.: Entität Beziehung Diagram) wird verwendet die Beziehungen von mehreren Entitäten zu Präsentieren.
### Entität
 Zu beginn an schauen was eine Entität ist. Eine Entität ist ein Objekt mit Information (z.B. eine Person) die auch Beziehungen haben kann mit Entitäten seiner eigenen Art oder mit anderen Entitäten (z.B. hat ein Auto, hat ein Haus).

### Notation
Ein ERD Diagramm hat sich die Symbolik ein bisschen über die Zeit geändert, aber in unseren fall (im falle der IHK) verwenden wir die Originale Chen-Notation von 1976.

*Hier ist ein Beispiel eines ERD Diagramms nach Chen zum beschreiben von Mitarbeitern und deren Abteilung:*
![ERD-Besipiel-1](ERD-Besipiel-1.svg)

Wir beschreiben jetzt anhand des Beispiels  den Aufbau eines ER Diagramms. Beginnen wir mit der Symbolik.
In einem ER Diagramm gibt es 3 Symbole die man verwenden kann.
1. Die Entität (Quadrat)
   Die Entität beschreibt das Objekt welches Beziehungen hat
2. Beziehung (Rhombus (Gedrehte Parallelogramm))
   Das Beschreibt die Beziehung von zwei Entitäten.
3. Attribut (Elipse)
   Ein Attribut ist weitere Information die eine Entität oder Beziehungen haben kann.

Nun schauen wir die Verbindungen an. Die erste Verbindung die wir anschauen ist die Verbindung zwischen Einer Entität/Beziehung und einem Attribut. Diese Beziehung wird mit einer einfachen Linie Designiert und beschreibt dass das zum Diagramm dazugehört

Als Nächstes betrachten wir die Beziehung zwischen einer Entität und einer Beziehung. Eine Beziehung verbindet immer zwei Entitäten und wird mit einer einfachen Linie verbunden, aber mann muss beachten das die Linien Notierungen haben. Diese Linien Beschriftungen beschreiben einer der 3 Beziehung arten.

| Beziehung | Beschreibung                                                                                                                                                                                                                |
| --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1-1       | Eine Eins zu Eins Beziehung beschreibt das Entität 1 und Entität zwei jeweilig min **nur** einen vom anderen eine Beziehung hat. z.B. Eine Person hat nur eine Leber und jede Leber hat nur eine Person                     |
| 1-n       | Eine eins zu N oder eins zu mehreren Beziehung beschreibt die wenn ein Entität eine beziehung mit meheren von einer entität haben kann. z.B. Eine Abteilung hat Mehrere Mitarbeiter aber ein Mitarbeiter hat eine Abteilung |
| n-m       | Eine N zu M oder Mehrere zu Mehrere Beziehung beshreibt wenn eine Entität eine Bezhiung mit mehreren Version von einer Entität und umgekehrt                                                                                |
### Übertragen in eine Relationale Datenbank 
Um es in eine Realationale Datenbank zu konvertieren is relative einfache. Jede Entität ist eine Tabelle mit den Spalten der Attribute. Die Beziehungen werden mit Foraign Key, in die jeweiligen Tabellen verbunden. Ausnahmen sind *N zu M* Beziehungen oder Beziehungen mit Attributen die eine Zwischen Tabelle benötigen.

### Weitere Referencen
- [Entity–relationship model - Wikipedia](https://en.wikipedia.org/wiki/Entity%E2%80%93relationship_model)
- [Chen Notation | Vertabelo Database Modeler](https://vertabelo.com/blog/chen-erd-notation/)
