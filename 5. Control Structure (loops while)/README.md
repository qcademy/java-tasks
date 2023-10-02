# While Loop

Video: [Java: While loop](https://www.youtube.com/watch?v=rt2daYZYlwM)

## Aufgabe 1
**A)** Welche Unterschiede gibt es zwischen While und for- Schleifen?

**B)** Schreiben folgendes Snippet anhand einer While Schleife um:
```java
for (int i = 0; i < 10; i++) {
    if ((i%2) == 0) {
        System.out.println(i + " ist eine gerade Zahl")
    } else {
    System.out.println(i + " ist eine ungerade Zahl");
    }
}
```
**C)** Beschreiben was die folgende Funktion macht:
```java
public static void func(int n) {
    int m = n + 1;
    while (true) {
        if ((m % n) == 0) {
            m ++;
            continue;
        }
        m ++;
        System.out.println("m = " + m);
    }
}
```

## Aufgabe 2
Ergänzen Sie folgende Funktion, so dass die Summe der im Array **arr** enthaltenen
Zahlen berechnet wird. Verwenden Sie dafür eine While Schleife.
```java
public static double array_summe(double[] arr) {
    // TODO: Summe implementieren
}
```
Überprüfen Sie Ihre eigene Implementierung anhand von Aufrufen in einer main
Methode.

## Aufgabe 3
Implementieren Sie die Funktion primeNumbers, sodass alle Primzahlen bis n
(inklusiv) auf der Konsole ausgegeben werden. Die Signatur der Funktion ist wie
folgt:
```java
public static void primeNumbers(int n);
```
Falls eine Schleife benötigt wird, dann verwenden Sie eine While Schleife.
Überprüfen Sie Ihre eigene Implementierung anhand von Aufrufen in einer main
Methode.

## Aufgabe 4
Implementieren die Funktionen ggt, die den größten gemeinsamen Teiler von 2
ganzen Zahlen zurückgibt. Die Signatur der Funktion ist wie folgt:
```java
public static int ggt(int n, int m);
```
Überprüfen Sie Ihre eigene Implementierung anhand von Aufrufen in einer main
Methode.