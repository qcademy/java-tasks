# Control structures

Video: [Java: Kontrollstrukturen(if else, switch)](https://www.youtube.com/watch?v=GYdn6E69fWs)

## Aufgabe-1
Gegeben seien folgende Code Zeilen:
```java
if (a > 2 == true) { 
    System.out.println("a ist groesser als 2"); 
}
```
und:

```java
if (a > 2) { 
    System.out.println("a ist groesser als 2"); 
}
```

Erklären Sie warum beide Zeilen gleich sind(im Sinne der Auswertung). Welche
Variante bevorzugen Sie und warum ?

## Aufgabe-2
**A)** Gegeben sei folgendes Snippet(Stück Code):
```java
...
if (a == 0) {
    System.out.println("a ist gleich 0");
} else if (a == 2) {
    System.out.println("a ist gleich 2");
} else if (a == 3) {
    System.out.println("a ist gleich 3");
} else if (a == 7) {
    System.out.println("a ist gleich 7");
} else {
    System.out.println("Der Wert von a ist unerwartet");
}
...
```
Optimieren Sie dieses Snippet durch die Verwendung der Kontrollstruktur: switch

**B)** Schreiben Sie folgendes Snippet anhand des **if else** Konstrukts um:
```java
...
return a > 2 ? 42 : a < 15 ? 18 : 90;
...
```
Was sind die Vor- und Nachteile der umgeschriebenen Form ?

**C)** Optimieren Sie folgendes Snippets, indem Sie ein geeigneteres Konstrukt
einsetzen
```java
...
switch(a) {
    case 13:
        return 32;
    default:
        return 78;
}
...
```

**D)** Gegeben sei folgendes Snippet. Beschreiben Sie in Ihren eigenen Worten, was in
diesem Code passiert
```java
...
switch(a) {
    case 42:
        break;
    case 52:
    case 11:
        System.out.println("Programmieren macht richtig Spass!");
        break;
    case 34:
        System.out.println("Hello World");
        break;
    default:
        System.out.println("Funny");
}
...
```

## Aufgabe-3
Gegeben sei folgendes Snippet ergänzen die statische Methode **summe**, so dass
diese die Summe aller **natürlichen Zahlen** von 1 bis n berechnet. Die Funktion
**summe** soll anhand einer Rekursion implementiert werden.
Rufen Sie die Funktion **summe** mehrfach mit verschiedenen Zahlen in der main
Methode auf und überprüfen die Richtigkeit Ihrer Implementierung.
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

## Aufgabe-4
Recherchieren Sie über die Definition der mathematischen Funktion Namens
**Fakultät** und Schreiben eine statische und rekursive Methode Namens **fakultaet**,
die die Fakultät einer als Parameter übergebenen natürlichen Zahl berechnet.
Überprüfen Sie die Richtigkeit Ihrer Implementierung.

## Aufgabe-5
Recherchieren Sie über die Definition von **Fibonacci Zahlen** und implementieren
Sie eine statische und rekursive Methode Namens **fibonacci**, die die Fibonacci Zahl
einer als Parameter übergebenen natürlichen Zahl berechnet.
Überprüfen Sie die Richtigkeit Ihrer Implementierung.
