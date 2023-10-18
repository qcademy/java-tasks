# OOP - Konstruktoren

Video: [Java: OOP - Konstruktoren](https://youtu.be/u_knK-nmwlQ)

## Aufgabe 1
**A)** Wozu dient der Konstruktor in einer Klasse?

**B)** Was bedeutet es einen Konstruktor zu überladen? 
Wie kann man einen Konstruktor in einem anderen aufrufen?

**C)** Was wird in der OOP unter einer factory Methode verstanden? 
Was ist der Unterschied zwischen einer solchen Methode und einem Konstruktor.

**D)** Was wird unter dem Begriff **interne Klasse** in Java verstanden?

## Aufgabe 2
Eine Firma vermietet für Gruppen, Vereine oder Privatpersonen eine Vielzahl von
Räumen in einem Hochhaus. Der Firma gehört das gesamte Hochhaus, es stehen
aber nicht immer alle Räume zur Verfügung. Um das Problem einfach zu halten,
gehen wir davon aus, dass die zur Verfügung stehenden Räume durchnummeriert
sind.
Für das Problem wurden folgende Parameter in einem Pflichtenheft festgehalten:
1. Von der Firma wird der Name, eine Adresse, die Anzahl der Räume zur
   Vermietung und die maximale Anzahl der möglichen Räume gespeichert.
2. Alle Attribute müssen gelesen werden können.
3. Die Größe der Räume (d. h. die Menge der Sitzplätze) wird in einem Feld
   gespeichert.
4. Die einzelnen Räume werden von Kunden gebucht, diese werden in einem
   Feld gespeichert.
5. Eine Firma wird mit ihrem Namen und der Adresse erzeugt, zudem werden
   alle notwendigen Werte gesetzt.
6. Es kann ein Raum (mit der Sitzplatzmenge) hinzugefügt werden.
7. Es muss eine Methode geben, die nach einem Raum mit einer gewünschten
   Größe sucht und dessen Nummer zurückgibt; findet sich kein Raum, wird -1
   zurückgegeben.
8. Es muss eine Methode geben, die die Anzahl der freien (ungebuchten)
   Räume ermittelt und zurückgibt.

Implementieren Sie:
- den **Konstruktor** der Klasse Firma,
- die Methode fuegeRaumHinzu(int plaetze),
- die Methode sucheRaum(int plaetze) und
- die Methode anzahlFrei().

## Aufgabe 3
Modellieren Sie eine Klasse Buch mit den Attributen titel, isbn und preis. Ein Buch
wird mit seiner isbn und seinem Titel erzeugt. Alle Attribute sollen gelesen werden
können, nur der Preis soll geändert werden können. Die Klasse besitzt eine Methode
toString, welche die Buchdaten zurückgibt.
Die Klasse Autor wird durch die Attribute name, synonym und gage gekennzeichnet.
Ein Autor wird mit seinem Namen erzeugt, alle Attribute können gelesen werden,
synonym und gage können auch gesetzt werden. Die Klasse Autor besitzt eine
Methode toString, welche die Daten des Autors zurückgibt.
Zu jedem Buch soll ein Autor gespeichert werden.

1. Beschreiben Sie, wie der Autor in der Klasse Buch durch Attribute und
   Methoden eingebunden wird.
2. Implementieren Sie die Klassen Buch und Autor in Java.
3. Implementieren Sie ein Java-Programm AppBuch, welches drei
   Bücher mit ihren Autoren erzeugt und über die Methode toString die
   Daten ausgibt.

## Aufgabe 4
Erweitern Sie das Java-Programm **AppBuch** aus der Aufgabe 3, so dass die
Attribute von Büchern aus der Konsole gelesen werden. Nach der Eingabe der
benötigten Attributen soll ein entsprechendes Buch erzeugt werden. Zur Bestätigung
der Erzeugung wird die String Darstellung des Buches auf der konsole ausgegeben,
bevor das Programm wieder im Eingabe-Modus übergeht(REPL). Die Ausgabe sollte
wie folgt aussehen: Buch: .... erzeugt.

Erweitern Sie Ihr Programm um eine Klasse Bibliothek. Eine Bibliothek sollte die
Möglichkeit bieten Bücher zu verwalten. Folgende Verwaltungsoperationen sollten
unterstützt werden:
- Buch hinzufügen
- Buch ausleihen
- Buch zurückgeben
- Buch löschen

Diese Operationen sollten aus der Konsole ausführbar sein.