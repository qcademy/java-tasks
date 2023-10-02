# For Loop

Video: [Java: For loop](https://www.youtube.com/watch?v=odYJFC6EDUU)

## Aufgabe 1
**A)** Beschreiben Sie in Ihren eigenen Worten, was man in der Programmierung
unter dem Begriff einer Schleife versteht.

**B)** Listen Sie auf und definieren Sie die wichtigsten Bestandteile einer
For-Schleife

**C)** Beschreiben Sie in ihrer eigenen Worten, was eine endlose Schleife ist. Was
ist generell die Ursache solcher Schleifen?

**D)** Gegeben sei folgendes Snippet
```java
for (int i = 0; ; i++) {
    System.out.println("i = " + i);
}
```
Ist diese Schleife endlos ? Begründen Sie Ihre Antwort.

**E)** Definieren das Nutzen der folgenden Schlüsselwörter bzgl. einer For-Schleife
- break
- continue

## Aufgabe 2
Gegeben sei folgendes Snippet ergänzen die statische Methode **summe**, so dass
diese die Summe aller **natürlichen Zahlen** von 1 bis n berechnet. Die Funktion
**summe** soll anhand einer For-Schleife implementiert werden.
Rufen Sie die Funktion **summe** mehrfach mit verschiedenen Zahlen in der main
Methode auf und überprüfen Sie die Richtigkeit Ihrer Implementierung.
```java
public class HelloWorld {
    
    public static int summe(int n) {
        // TODO: Implementierung
    }
    
    public static void main(String[] args) {
        // TODO: Funktion summe aufrufen und auf der Konsole ausgeben
    }
}
```

## Aufgabe 3
Implementieren Sie eine statische Methode Namens **fakultaet**, die die Fakultät einer
als Parameter übergebenen natürlichen Zahl berechnet. Die Funktion soll anhand
einer For-Schleife implementiert werden.
Überprüfen Sie die Richtigkeit Ihrer Implementierung.

## Aufgabe 4
Implementieren Sie eine statische Methode Namens **fibonacci**, die die Fibonacci
Zahl einer als Parameter übergebenen natürlichen Zahl berechnet. Die Funktion soll
anhand einer For-Schleife implementiert werden.
Überprüfen Sie die Richtigkeit Ihrer Implementierung.