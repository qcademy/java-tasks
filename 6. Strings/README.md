# Strings

Video: [Java: Strings](https://www.youtube.com/watch?v=5GuzRsGKjGM)

# Aufgabe 1
**A)** Definieren Sie in Ihren eigenen Worten was in der Programmierung unter der
Bezeichnung **String** verstanden wird.

**B)** Definieren Sie in Ihren eigenen Worten was eine **String concatenation** ist
und geben ein Beispiel an.

**C)** Beschreiben Sie welche interne Schritte ausgeführt werden, wenn eine **String
concatenation** ausgeführt wird. Welche Nachteile sehen Sie daran und wie
könnten Sie diese vermeiden?

**D)** Was ist der Unterschied zwischen StringBuilder und StringBuffer?

**E)** Gegeben sei folgendes Snippet:
```java
...
String result = "";
for(int i = 0; i < 10000; i++) {
    result += generateRandomString()
}
...
```
Optimieren Sie diesen Code.

## Aufgabe 2
Implementieren Sie eine statische Methode **revert**, die ein als Parameter
übergebenes String Object umkehrt. Folgender Aufruf **revert("test")** z.B. sollte
folgendes ausgeben **"tset"**.
- Verwenden Sie keine der folgenden Klassen bzw. Möglichkeiten:
  - StringBuilder
  - StringBuffer
  - String Library als Dependency
- Verwenden Sie die folgende Signatur für die Methode:
```java
public static String revert(String str) {}
```

## Aufgabe 3
Implementieren Sie eine statische Methode **monthAsString**. Dieser Methode soll
ein String object im Format **"dd.mm.yyyy"** übergeben werden können.
Anschließend soll die Methode den Monat als String ausgeschrieben(deutsche
Sprache) zurückgeben.
Der Aufruf **monthAsString("06.09.2098")** sollte z.B. **"September"** als Ergebnis
zurückgeben.
Verwenden Sie die folgende Signatur für die Methode:
```java
public static String monthAsString(String str) {}
```

## Aufgabe 4
Ein Anagramm ist ein Satz, der durch Umstellen aller Buchstaben eines anderen
Satzes gebildet werden kann. Gross- und Kleinschreibung wird dabei ignoriert.
Ebenso spielen Leerzeichen keine Rolle. Aus dem Wort **"Desperation"** läßt sich zum
Beispiel der Satz **"A Rope Ends It"** bilden.
Implementieren eine statische Methode **isAnagram**, mit der zwei Zeichenketten
daraufhin überprüft werden können, ob sie ein Anagram bilden.
Verwenden Sie die folgende Signatur für die Methode:
public static boolean isAnagram(String str)

## Aufgabe 5
Implementieren Sie eine statische Methode palindrom, die aus einem Text alle
Palindrome auf der Konsole ausgibt. Folgender Aufruf
**palindrom("Der vor dir stehende Rentner heißt Otto Uwe")** sollte z.B. folgendes
auf der Konsole ausgeben:
```
Rentner
Otto
```
Verwenden Sie die folgende Signatur für die Methode:
```java
public static void palindrom(String text) {}
```