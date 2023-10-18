# Generics

## Aufgabe 1
Die Programmiererin Ursula S. soll eine Menge geometrischer Figuren wie z.B.
Kreise und Rechtecke in einer gemeinsamen Liste verwalten. Die Liste muss später
auch andere Figuren wie z.B. Dreiecke oder Rauten aufnehmen können.
Helfen Sie ihr und implementieren Sie je eine Klasse für Kreise und Rechtecke
sowie eine Klasse FigurenListe zur Verwaltung der Figuren mit den im Folgenden
beschriebenen Eigenschaften:
- Die Figuren Objekte sollen jeweils über eine Methode anzeigen zur
Darstellung der Figur verfugen.
- Die Darstellung einer Figur soll hier nur durch Ausgabe des Textes ”Kreis
anzeigen“, ”Rechteck anzeigen“ etc. auf der Konsole simuliert werden.
(Instanzvariablen wie z.B. der Kreismittelpunkt müssen nicht deklariert
werden.)
- Die Klasse FigurenListe soll ein Attribut figurenListe vom Typ **Array** für einen 
**generischen** Elementtyp **A** enthalten. Dieser Elementtyp muss sicherstellen,
dass in der Liste **nur Figuren** mit den angegebenen Eigenschaften
gespeichert werden können.
- Die Klasse FigurenListe soll die Methoden figurAnfuegen, letzteFigurAuslesen
und alleAnzeigen zur Verfugung stellen:
  - Mit Hilfe der Methode figurAnfuegen soll ein Figuren Objekt am Ende
  von figurenListe eingefügt werden.
  - Die Methode letzteFigurAuslesen soll das letzte gespeicherte
  Figurenobjekt zurückgeben.
  - Mit Hilfe der Methode alleAnzeigen können alle Elemente der Liste
  nacheinander am Bildschirm angezeigt werden.

## Aufgabe 2
Gegeben sei folgendes Code Snippet. Implementieren Sie die Methoden der Klasse
LocalList entsprechend der spezifizierten Anforderungen.
package de.qcademy.java.kurs;

```java
public class LocalList<A> {
    
    /**
     * Dieses Array soll verwendet werden, um Elemente der Liste zu speichern.
     */
    private final A[] speicher;
    
    /**
     * Durch diesen Konstruktor soll eine Leere(leerer Speicher) Liste erzeugt werden.
     */
    public LocalList();
    
    /**
     * Diese Methode soll die Länge der Liste zurückgeben.
     */
    public int size();
    
    /**
     * Diese Methode soll true zurückgeben when die Liste leer ist, ansonsten false.
     */
    public boolean isEmpty();
    
    /**
     * Diese Methode soll überprüfen, ob ein als Parameter übergebenes
     * Object in der Liste enthalten ist. Das Ergebnis soll als boolean zurückgegeben werden.
     */
    public boolean contains(Object o);
    
    /**
     * Diese Methode soll ein als Parameter übergebenes Object in der Liste hinzufügen.
     * True wird zurückgegeben wenn das Hinzufügen erfolgreich war.
     */
    public boolean add(A a);
    
    /**
     * Diese Methode soll ein Object aus der Liste löschen.
     * True wird zurückgegeben wenn das Löschen erfolgreich war.
     */
    public boolean remove(Object o);
    
    /**
     * Diese Methode soll überprüfen, ob als Parameter übergebene Objekte(ll)
     * in der Liste enthalten ist.
     * True wird zurückgegeben, ob alle übergebene Objekte in der Liste enthalten sind
     */
    public boolean containsAll(LocalList<A> ll);
    
    /**
     * Diese Methode soll als Parameter übergebene Objekte in der Liste hinzufügen.
     * True wird zurückgegeben, wenn das Hinzufügen erfolgreich war.
     */
    public boolean addAll(LocalList<A> ll);
    
    /**
     * Diese Methode soll Objekte an der stelle index in der Liste hinzufügen.
     * true wird zurückgegeben, wenn das Hinzufügen erfolgreich war.
     */
    public boolean addAll(int index, LocalList<A> ll);
    
    /**
     * Diese Methode soll Objekte aus der Liste löschen.
     * True wird zurückgegeben, wenn das Löschen erfolgreich war.
     */
    public boolean removeAll(LocalList<A> ll);
    
    /**
     * Diese Methode soll den internen Speicher zurücksetzen.
     */
    public void clear();
    
    /**
     * Diese Methode soll das Element an der Stelle index zurückgeben.
     */
    public A get(int index);
    
    /**
     * Diese Methode soll das Element an der Stelle index löschen.
     */
    public A remove(int index);
    
    /**
     * Diese Methode gibt eine Teilliste zurück.
     * Diese Teilliste soll Elemente von der Stelle a bis b(exklusiv) enthalten.
     */
    public LocalList<A> subList(int a, int b);
}
```
Testen Sie Ihre Implementierung in einer geeignete main Methode.