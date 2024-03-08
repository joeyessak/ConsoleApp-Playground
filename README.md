# Playground - Strings
## C# Strings
A string is an object of type String whose value is text. Internally, the text is stored as a sequential read-only collection of Char objects. There's no null-terminating character at the end of a C# string; therefore a C# string can contain any number of embedded null characters ('\0'). The Length property of a string represents the number of Char objects it contains, not the number of Unicode characters. To access the individual Unicode code points in a string, use the StringInfo object.

## string vs. Stystem.String
In C#, the string keyword is an alias for String; therefore, String and string are equivalent. It's recommended to use the provided alias string as it works even without using System;. The String class provides many methods for safely creating, manipulating, and comparing strings. In addition, the C# language overloads some operators to simplify common string operations.

## Immutability of strings
String objects are immutable: they can't be changed after they've been created. All of the String methods and C# operators that appear to modify a string actually return the results in a new string object.
<br></br>
Because a string "modification" is actually a new string creation, you must use caution when you create references to strings. If you create a reference to a string, and then "modify" the original string, the reference will continue to point to the original object instead of the new object that was created when the string was modified.

