# OOP - Vererbung

Video: [Java: OOP - Vererbung](https://youtu.be/Jv_K168dHIA)

## Aufgabe 1
**A)** Was versteht man in der OOP unter dem Begriff Vererbung?

**B)** Definiere in deinen eigenen Worten, was eine Generalisierung ist?

**C)** Definiere die folgenden Begriffe:
- Oberklasse
- Unterklasse

**D)** Definiere, was eine abstrakte Klasse ist.

**E)** Definiere, was eine abstrakte Methode ist.

## Aufgabe 2
Für die Simulation eines Wettrennens sollen verschiedene Fahrzeugarten
objektorientiert modelliert werden. Da alle Fahrzeugtypen gemeinsame
Eigenschaften haben, definieren wir uns zunächst eine Basis- und abstrakte Klasse
Fahrzeug, die als Oberklasse für die anderen Klassen dienen soll. Ein Fahrzeug hat
folgende allgemeinen Merkmale:
- Seine aktuelle Position (in km und der Einfachheit halber in nur einer
Dimension)
- Seine aktuelle Geschwindigkeit (in km/h)
- Es kann bewegt werden (Methode *_bewege_*). Die Methode wird mit
einem Double Parameter aufgerufen, der die Anzahl der Minuten
angibt, in denen das Fahrzeug mit der aktuellen Geschwindigkeit fährt.
Der Methodenaufruf ändert natürlich die Position des Fahrzeugs, wenn
es mit einer von 0 verschiedenen Geschwindigkeit bewegt wird.
- Man kann seine Geschwindigkeit setzen (Methode
*_setzeGeschwindigkeit_*). Die Geschwindigkeit darf die
Maximalgeschwindigkeit nicht überschreiten.
- Es kann seine Maximalgeschwindigkeit angeben (Methode
*_getMaxGeschwindigkeit_*). Für ein Objekt der Klasse Fahrzeug soll die
Maximalgeschwindigkeit 0 sein.
- Es kann die Anzahl seiner Räder angeben. In der Klasse Fahrzeug soll
diese ebenfalls 0 sein.

Nun sollen einige konkrete Fahrzeuge definiert werden, indem entsprechende
Klassen von Fahrzeug abgeleitet werden:

- Ein **Fahrrad** ist ein Fahrzeug mit 2 Rädern und
Maximalgeschwindigkeit 30 km/h.
- Ein **Auto** ist ein Fahrzeug mit 4 Rädern und Maximalgeschwindigkeit
140 km/h.
- Ein **Rennwagen** ist ein Auto mit Maximalgeschwindigkeit 220 km/h.
- Ein **Krankenwagen** ist ein Auto mit einem zusätzlichen Blaulicht, das
ein- oder ausgeschaltet sein kann (neues Attribut!). Außerdem muss
der Krankenwagen Methoden zum Ein- bzw. Ausschalten des
Blaulichts anbieten.

Definiere diese Klassen und nutze dabei so weit wie möglich die Vererbung von
Eigenschaften aus!