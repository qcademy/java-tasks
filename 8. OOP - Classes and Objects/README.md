# OOP - Klassen und Objekte

Video: [Java: OOP - Klassen und Objekte](https://youtu.be/K2v2skZzQYw)

## Aufgabe 1
**A)** Definieren Sie, was eine Klasse in der OOP ist. Wie wird eine Klasse in Java
deklariert?

**B)** Definieren Sie, was ein Objekt in der OOP ist. Wie wird ein Objekt in Java
erzeugt?

**C)** Welche Unterschiede gibt es zwischen einer Instanz und einem Objekt einer
Klasse?

**D)** Was versteht man in der OOP unter Konstruktor. Wie wird ein Konstruktor
deklariert und aufgebaut?

**E)** Was versteht man unter statischen Attributen in der OOP?

**F)** Definieren Sie die folgenden Sichtbarkeiten in Java
- Private
- Protected
- Public
- Package private

## Aufgabe 2
Modellieren Sie Auto als Klasse nach den folgenden Festlegungen:
- Zu einem Auto werden KFZ-Kennzeichen, Kilometerstand, Tankvolumen,
Kraftstoffverbrauch und Kraftstoffmenge erfasst.
- Ein Auto kann tanken(Menge) und fahren(Strecke).
- Die aktuellen Werte der Attribute KFZ-Kennzeichen, Kilometerstand und
Tankvolumen können abgefragt werden.
- Ein Auto soll sowohl ohne Werte als auch mit geeigneten Startwerten erzeugt
werden können.

Implementieren Sie die Klasse Auto in Java.

Implementieren Sie eine Klasse AppAuto, in der zwei Autos erzeugt werden und
diese fahren bzw. tanken.

## Aufgabe 3
Schreiben Sie eine Klasse, die ein Bankkonto realisiert. Attribute für das Bankkonto
sind der Name und Vorname des Kontoinhabers, die Kontonummer, der Kontostand
sowie ein Limit, bis zu dem das Konto überzogen werden darf.

1. Erstellen Sie einen oder mehrere geeignete Konstruktoren
2. Erstellen Sie Methoden für folgende Operationen:
   1. Ausgabe der Kontodaten (toString())
   2. Einzahlung
   3. Auszahlung
   4. Abfrage des Kontostandes

## Aufgabe 4
Die Klasse Punkt soll einen Punkt in einem zweidimensionalen Koordinatensystem
repräsentieren. Ein Punkt besteht aus folgenden Attribute:
- X-Koordinate
- Y-Koordinate

Die Klasse Punkt soll Methoden für folgende Problemfelder erhalten:
- toString()
- Abstand des Punktes zum Ursprung
- Spiegelung des Punktes an der X-Achse (Ergebnis soll ein neuer Punkt sein)
- Spiegelung des Punktes an der Y-Achse (Ergebnis soll ein neuer Punkt sein)
- Spiegelung des Punktes am Ursprung (Ergebnis soll ein neuer Punkt sein)
- Abstand des Punktes zu einem anderen Punkt

Implementieren Sie die Klasse Punkt in Java und testen Sie diese mit einer Klasse
AppPunkt.

## Aufgabe 5
Implementieren Sie eine Klasse Radio mit folgenden Attributen:
- eingeschaltet, wenn ein Radio an oder aus ist
- Lautstärke, wie laut spielt das Radio Musik ? (Die Lautstärke soll nur im
Bereich von 0 bis 10 liegen)
- Frequenz, die die Frequenz des gewählten Senders angibt (Erlaubter
Frequenzbereich ist zwischen 85.0 und 110.0)

Implementieren Sie eine Klasse Radio mit folgenden Attributen:
- Radio()
- Radio(boolean istAn, int lautstaerke, double frequenz)

Zu der Klasse Radio sollen folgende Methoden implementiert werden:
- lauter(), leiser(): Diese Methoden sollen die Lautstärke ändern(nur möglich im
Zustand an)
- an(), aus(): Diese Methoden sollen den Zustand des Attributs **eingeschaltet**
ändern.
- public String toString(): Diese Methode soll Informationen über den internen
Zustand als String zurückgeben. Es soll eine Zeichenkette der form:
,,Radio an: Freq: 98.4, Laut=2’’ zurückgeben.
- waehleSender(double frequenz): Diese Methode eine Frequenz speichern. Ist
die gewählte Frequenz außerhalb der erlaubten Frequenzbereichs, so soll die
Frequenz 99.9 gewählt werden