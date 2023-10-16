# Java Code Conventions

## Formatting
A `.java` source file should be structured as follows:
1. Package declaration;
2. Import statements;
3. Class declaration;

There may be only one top level class declaration per file.

## Class Structure
The recommended order of class members is the following:
1. Fields;
2. Constructors;
3. Factory methods;
4. Other Methods;

Related fields should be grouped together. Ordering fields primarily according to access modifiers or identifier is not required.
The same applies to methods.

## Braces
Opening braces should be put on the end of the current line rather than on a line by its own.
There should be a new line in front of a closing brace unless the block is empty (see Short Forms below)
Braces are recommended even where the language makes them optional, such as single-line if and loop bodies.
- If a block spans more than one line (including comments) it must have braces;
- If one of the blocks in a `if / else` statement has braces, the other block must too;
- If the block comes last in an enclosing block, it must have braces;

The `else, catch` and the `while` keyword in `do…while` loops go on the same line as the closing brace of the preceding block.

**&check; Dos:** 
```java
void method() {
    ...
}
```
```java
try {
    something();
} catch (AnException e) {
    ...
}
```
```java
for (int[] row : matrix) {
    for (int val : row) {
        sum += val;
    }
}
```
**&cross; Don'ts:**

```java
// Wrong placement of opening brace
void method()
{
    ...
}
```
```java
// Newline in front of catch should be avoided
try {
    something();
}
catch (AnException e) {
    ...
}
```
```java
// Braces should be used
if (flag)
    // Restore x
    x = 1;

```
## Whitespace
### Vertical Whitespace
A single blank line should be used to separate:
- Package declaration;
- Class declarations;
- Constructors;
- Methods;
- Static initializers;
- Instance initializers;

and may be used to separate logical groups of
- import statements;
- fields;
- statements;

Multiple consecutive blank lines should not be used in your code.
### Horizontal Whitespace
A single space should be used:
- To separate keywords from neighboring opening or closing brackets and braces;
- Before and after all binary operators and operator like symbols such as arrows in lambda expressions and the colon in 
enhanced for loops (but not before the colon of a label);
- After `//` that starts a comment;
- After commas separating arguments and semicolons separating the parts of a for loop.
- After the closing parenthesis of a cast;

In variable declarations it is not recommended to align types and variables.

**&check; Dos:**
```java
int someInt;
String myString;
char aChar;
long sixtyfourFlags;
```
```java
if (isFlagSet(GO)) {
    ...
}
```
```java
IntUnaryOperator inc = x -> x + 1;
```
**&cross; Don'ts:**
```java
int    someInt;
String myString;
char   aChar;
long   sixtyfourFlags;
```
```java
if( isFlagSet( GO ) ) {
    ...
}
```
```java
IntUnaryOperator inc = x->x + 1;
```

## Naming Rules
The below list outlines the standard Java naming conventions for each identifier type:

### Packages:
Names should be in lowercase without underscores or other special characters, don’t use plural form. Normally should be subdivided. 
Typically this will start with the company domain before being split into layers or features:
```java
package de.qcademy.java;
```

### Classes:
Names should be in CamelCase. Try to use nouns because a class is normally representing something in the real world.
Use whole words and avoid using abbreviations unless the abbreviation is more widely used than the long form:

**&check; Dos:**
```java
class Customer {
    ...
}
```
```java
class EmptyCell {
    ...
}
```
```java
class XmlParser {
    ...
}
```

**&cross; Don'ts:**
```java
class customer {
    ...
}
```
```java
class Empty {
    ...
}
```
```java
// Abbreviation should be formatted as 'Xml'
class XMLParser {
    ...
}
```
### Interfaces: 
Names should be in CamelCase. They tend to have a name that describes an operation that a class can do:
```java
interface Comparable {
    ...
}
```
### Methods:
Names should be in mixed case (same as CamelCase except the first letter of the name is in lowercase). Use verbs to 
describe what the method does:

**&check; Dos:**
```java
public void expand() {
    ...
}
```
```java
public State getState() {
    ...
}
```
```java
public boolean isExpanding() {
    ...
}
```
**&cross; Don'ts:**
```java
public boolean expanding() {
    ...
}
```
```java
public State GetState() {
    ...
}
```
```java
public int get_index() {
    ...
}
```
### Variables:
Names should be in mixed case. The names should represent what the value of the variable represents:

**&check; Dos:**
```java
String firstName;
int orderNumber;
```
**&cross; Don'ts:**
```java
String first_name;
int OrderNumber;
```
Only use very short names when the variables are short-lived, such as in for loops:
```java
for (int i=0; i<20;i++) {   
    // i only lives in here 
}
```
### Constants:
Names should be in uppercase.
```java
static final int DEFAULT_WIDTH = 10;
```

## Commenting Code
First and foremost, try to make the code simple enough that it’s self explanatory. While comments explaining the code are good, 
not having to explain the code is better.
For single line comments, use end-of-line comments (`//`) otherwise use multiline comments (`/* … */`).
Small well documented methods are preferred over longer methods with comments in the body of the method.
Don’t push code that’s commented out.
Comments should be grammatically correct and follow general recommendations of technical writing.

## Code Formatting
We are not using a specific code style format, please use default Intellij IDEA formatting by selecting the code (Ctrl + A) 
and pressing the following combination on the keyboard:
- Windows: ```Ctrl + Alt + L```
- Mac OS: ```Command + Option + L```
