# Java Operatoren

Videos: 
- [Java: Definition of Java operators](https://youtu.be/h8_BDE6hns8)
- [Java: Practical examples](https://youtu.be/I8d_CZW5IS8)

## Aufgabe-1
Definieren Sie in Ihren eigenen Worten die folgenden Java Operator Typen:
- Arithmetische Operatoren
- Logische Operatoren
- Zuweisungsoperatoren
- Vergleichsoperatoren
- Cast Operator

Für jeden dieser Typen geben Sie mind. einen Operator an.

## Aufgabe-2
**A)** Gegeben seien folgende Code Zeilen. Lassen sich beide Zeilen kompilieren?
Begründen Sie Ihre Antwort.
1) `int a = 93/2;`
2) `int b = 93.0/2;`

**B)** Welche Operatoren Lassen sich auf Chars (Character) anwenden ? Geben
Sie für jeden Operator ein Beispiel an.

**C)** Gegeben sei folgende Code Zeile.
```java
int a = 21;
```
Was würde die Ausführung der folgenden Codezeilen auf der Konsole
ausgeben ?
1) `System.out.println(++a);`
2) `System.out.println(a++);`
3) `System.out.println(a%9);`
4) `System.out.println(a < 3);`

**D)** Welche Werte haben die folgenden Variablen
1) `boolean b1 =! true;`
2) `boolean b2 = (3 > 3) && ((2 == 2) || (4 > 90));`
3) `boolean b3 = (45 != 9) & ! true;`

**E)** Gegeben sei folgendes Stück Code. Beschreiben Sie was in Zeile 3 geschieht
und erklären Sie dabei, warum der Code sich kompilieren lässt, obwohl die
Division einen **Double-Wert** zurückgibt.
```java
public class HelloWord {
    public static void main(String[] args) {
        int a = (int) 92.4/3;
    }
}
```