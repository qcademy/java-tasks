# OOP - Interfaces

Video: [Java: OOP - Interfaces](https://youtu.be/JaEYZFszXmI)

# Aufgabe 1
**A)** Definiere in deinen eigenen Worten, was ein Interface ist.

**B)** Was ist der Unterschied zwischen abstrakten Klassen und Interfaces in Java?

**C)** Was eine default Methode in Java Interfaces?

**D)** Was ist eine anonyme Interface Implementierung?

**E)** Was ist ein funktionales Interface in Java?

## Aufgabe 2
Schaue Dir das folgende Interface sowie die beiden folgenden Klasse an:
```java
interface Vergleichbar {
    /**
    * vergleicht das aufgerufene Objekt mit dem als Parameter uebergebenen
    * Objekt; liefert: -1 falls das aufgerufene Objekt kleiner ist als das
    * Parameterobjekt 0 falls beide Objekte gleich gross sind 1 falls das
    * aufgerufene Objekt groesser ist als das Parameterobj.
    */
  int vergleichenMit(Vergleichbar obj);

}

class NuetzlicheFunktionen {
    /**
     * liefert ein "kleinstes" (auf der Basis der
     * Vergleichbar-Implementierung!) Element des Parameter-Arrays
     * Achtung: Man kann davon ausgehen, dass das Parameter-Array
     * mindestens 1 Element enthaelt
     */
    
    public static Vergleichbar kleinstesElement(Vergleichbar[] elemente) {
        // todo
    }
}

class Integer {
    protected int wert;
    
    public Integer(int w) {
        this.wert = w;
    }
    
    public int getWert() {
        return this.wert;
    }
}

```

1. Implementiere die Methode kleinstesElement der Klasse NuetzlicheFunktionen.
2. Leite von der Klasse Integer eine Klasse VInteger ab, die das Interface
   Vergleichbar implementiert.
3. Schreibe ein kleines Testprogramm, das zunächst ein Array mit VIntage
   Objekten erzeugt und initialisiert, anschließend die Funktion kleinstesElement
   mit diesem Array aufruft und den Wert des ermittelten kleinsten Elements auf
   den Bildschirm ausgibt.

## Aufgabe 3
In dieser Aufgabe geht es um die Verschlüsselung von Texten. Klartexte über einem
Klartext-Alphabet werden durch die Anwendung von Verschlüsselungsalgorithmen in
Geheimtexte über ein Geheimtextalphabet überführt. Verschlüsselungsverfahren
sollen gewährleisten, dass nur Befugte bestimmte Botschaften lesen können.
Schaue Dir dazu das folgende Interface an:
```java
  interface Chiffrierung {
    char chiffrieren(char zeichen);
    char dechiffrieren(char zeichen);
}
```

Das Chiffrieren ist ein Verschlüsselungsverfahren, bei dem jeder Buchstabe in einem
Text durch einen anderen Buchstaben ersetzt wird. Die Methode chiffrieren des
Interfaces soll eine entsprechende Umsetzung des übergebenen Zeichen
vornehmen. Die Methode _**dechiffrieren**_ bildet die umgekehrte Funktion.
Deine Aufgabe besteht nun darin, das Interface zweimal zu implementieren:
- Bei der ersten Implementierung solltest Du die sogenannte Caesar
Verschiebung implementieren. Die Caesar-Verschiebung beruht auf einem
Geheimtextalphabet, das um eine bestimmte Stellenzahl n gegenüber dem
Klartext Alphabet verschoben ist. Beispiel für `n = 3: a -> d, b -> e, c -> f, ..., w -> z, x -> a, y -> b, z -> c`. 
Chiffriert werden sollen hier nur Kleinbuchstaben.
Alle anderen Zeichen sollen unverändert zurückgegeben werden.
Implementiere neben den beiden Methoden des Interfaces einen Konstruktor,
dem die Stellenzahl als Parameter übergeben wird.
- Bei der zweiten Implementierung des Interface übergebe im Konstruktor
explizit das Geheimtextalphabet als 26 elementiges char-Array m. Die
Chiffrierung erfolgt hierbei durch: `a -> m[0], b -> m[1], ..., z -> m[25]`. Chiffriert
werden sollen auch hier nur Kleinbuchstaben. Alle anderen Zeichen sollen
unverändert zurückgegeben werden.

Implementiere anschließend die folgende Klasse:
```java
public class Verschluesselung {
    public static String verschluesseln(String klartext, Chiffrierung schluessel);
    public static String entschluesseln(String geheimtext, Chiffrierung schluessel);
}
```
zum Ver- bzw. Entschlüsseln von Botschaften gemäß eines zwischen Sender und
Empfänger vereinbarten Chiffrierungsschlüssels.

Implementiere weiterhin **Unittests** für die Klasse Verschluesselung, und überprüfe
anhand deiner Testfälle, ob die oben genannten Chiffrierungsverfahren richtig
implementiert wurden.