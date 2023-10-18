# OOP - Methoden

Video: [Java: OOP - Methoden](https://youtu.be/f9YwVnIKpDw)

## Aufgabe 1
**A)** Beschreiben Sie die folgenden Begriffe
- Methode überladen
- Methode überschreiben
- Finale Methode

**B)** Was versteht man unter dem Begriff: Seiteneffekt?

**C)** Beschreiben Sie in Ihren eigenen Worten, was eine Seiteneffektfreie Klasse ist.

**D)** Beschreiben Sie in Ihren eigenen Worten, was eine statische Methode ist

## Aufgabe 2
Vor einer Autowaschanlage der Tankstelle „OSSE“ gibt es regelmäßig eine Schlange
an Autos, die gewaschen werden sollen. Die bekannte Firma ProfiSoft soll nun ein
Programm entwickeln, welches diese Warteschlange verwaltet. Aus
Erfahrungsgründen (und aus Platzgründen) sind nie mehr als 10 Autos in dieser
Schlange. Natürlich soll sich ein neu hinzukommendes Auto am Ende der Schlange
anstellen (solange noch Platz ist), außerdem sollen alle wartende Autos aufrücken,
wenn das an erster Stelle stehende Auto in die Anlage einfahren darf, Autos können
natürlich jederzeit die Schlange verlassen und wieder „nach Hause“ fahren.
1. Stellen Sie zu dem gegebenen Problem ein (geeignetes) Pflichtenheft
   auf. Suchen Sie sich dafür notwendige und sinnvolle Eigenschaften für
   die Klasse Auto
2. Modellieren Sie eine geeignete Klasse Auto.
3. Modellieren Sie eine geeignete Klasse Warteschlange. (Verwenden Sie
   zum Verwalten der gewünschten Anzahl an Autos eine geeignete
   Datenstruktur.)

## Aufgabe 3
Die Firma ProfiSoft erhält den Auftrag, ein Programm zur Verwaltung einer
Zahnarztpraxis zu entwickeln. Das vom Auftraggeber vorgegebene Pflichtenheft
sieht folgendermaßen aus:
1. Über jeden Kassen-Patienten sind folgende Daten zu speichern:
   Patienten-Nr., Patientenname, Adresse, Geburtsdatum,
   Versichertenname, Versicherten-Karte vorgelegt (ja, nein).
2. Jeder Kassen-Patient gehört zu genau einer Krankenkasse.
3. Jede Krankenkasse kann mehr als einen Kassen-Patienten haben.
4. Über jede Krankenkasse sind folgende Daten zu speichern:
   Kassennummer, Kassenname.
5. Wird ein neuer (Kassen-)Patient angelegt, dann sind die Patienten-Nr.
   und der Patientenname einzutragen.
   1. Gleichzeitig ist der neue Patient einer Krankenkasse
      zuzuordnen.
      1. Variante I: es gibt nur eine Krankenkasse (wurde vorher angelegt)
      2. Variante II: es gibt mehrere Krankenkassen (wurden vorher angelegt)
      3. Variante III: es wird überprüft, ob die angegebene Krankenkasse schon
        vorhanden ist; evtl. muss sie neu angelegt werden
6. Der Versichertenname ist mit dem Patientennamen beim Erzeugen
   vorzubelegen. „Versicherten-Karte vorgelegt“ ist mit „ja“ zu
   initialisieren.

Implementieren Sie das Pflichtenheft in einem lauffähigen Java-Programm. Testen
Sie die Klassen in einer geeigneten App; zunächst nur zwei Patienten und zwei
Kassen.