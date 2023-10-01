# Primitive Datentypen

## Aufgabe-1
Beschreiben Sie in Ihren eigenen Worten die folgenden Datentypen:
- boolean
- float
- byte
- int
- double
- char
- short
- long
- Object

Soweit möglich definieren für jeden dieser Datentypen den Definitionsbereich der
möglichen Werte.

## Aufgabe-2
Definieren Sie in Ihren eigenen Worten die folgenden Begriffe:
- Statische Typisierung
- Java Package
- Main Methode
- Variablen Deklaration
- Initialisierung einer Variable
- Immutable/finale Variablen

## Aufgabe-3
Definieren Sie in Ihren eigenen Worten, was man in der Programmierung unter
**Zuweisung** versteht. Ergänzen Sie die Hauptmethode des folgenden Stück Codes,
indem Sie für jeden der in [Aufgabe-1](#Aufgabe-1) aufgelisteten primitiven Datentypen eine
Beispiel Zuweisung (als unveränderliche Variable) machen:
```java
public class HelloWord {
    public static void main(String[] args) {
    // TODO: Hier Ihren Code schreiben
    }
}
```

##Aufgabe-4
Gegeben sei folgendes Stück Code. Beschreiben Sie warum dieser Code sich nicht
kompilieren lässt.
```java
public class HelloWord {
    public static void main(String[] args) {
        double a;
        int b = 42;
        b = a;
        System.out.println("Hello world " + a);
    }
}
```

Korrigieren Sie die Fehler, so dass der Code sich kompiliert lässt (IntelliJ, Maven).
Hinweis: Nach erfolgreicher Korrektur sollte der Code folgendes: **Hello world 42.0**
auf der Konsole ausgegeben werden.