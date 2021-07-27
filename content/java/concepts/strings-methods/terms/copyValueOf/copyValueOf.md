---
Title: "copyValueOf()"
Subjects:
  - "Computer Science"
Tags:
  - "Methods"
  - "Strings"
Catalog Content:
  - "https://www.codecademy.com/learn/learn-java"
  - "https://www.codecademy.com/learn/paths/computer-science"
---

## Definition

Returns a string with characters copied from an array.

## Syntax

```java
public String copyValueOf(char[] data, int offset, int count)
```

- `data` (required): An array of characters to be copied from.
- `offset` (optional): The index of the first character to be copied.
- `count` (optional): The number of characters to be copied.

## Example 1

Copy all characters from the array `charactersArray` to the string `copiedCharacters`:

```java
class CopyAllCharacters {
  public static void main(String[] args) {
    String copiedCharacters = "This string will be replaced with copied characters.";
    char[] charactersArray = {'a','b','c','d','e'};
    System.out.println(copiedCharacters.copyValueOf(charactersArray));
    // Output: abcde
  }
}
```

## Example 2

Copy two characters from the array, starting at index `4`:

```java
class SpecificCharactersToCopy {
  public static void main(String[] args) {
    String copiedCharacters = "This string will be replaced with copied characters.";
    char[] charactersArray = {'a','b','c','d','e','f','g','h','i'};
    System.out.println(copiedCharacters.copyValueOf(charactersArray, 4, 2));
    // Output: ef
  }
}
```