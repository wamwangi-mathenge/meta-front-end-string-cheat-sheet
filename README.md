# String Cheat Sheet

By the end of this reading, you'll be able to:
- Identify examples of String functions and explain how to call them

This doc lists some of the most common and most useful properties and methods available on strings.

All strings have at their disposal several built-in properties, but there's a single property that is really useful: the length property:

~~~
var greet = "Hello, ";
greet.length; // 7
~~~

To read each individual character at a specific index in a string, starting from zero, you can use the charAt() method:

~~~
greet.charAt(0); // 'H'
~~~
The concat() method joins two strings:  
~~~
"Wo".concat("rl").concat("d"); // 'World'
~~~

The indexOf returns the location of the first position that matches a character:
~~~
"ho-ho-ho".indexOf('h'); // 0
"ho-ho-ho".indexOf('o'); // 1
"ho-ho-ho".indexOf('-'); // 2
~~~

The lastIndexOf finds the last match, otherwise it works the same as indexOf.

The split method chops up the string into an array of substrings:
~~~
"ho-ho-ho".split("-"); // ['ho', 'ho', 'ho']
~~~

There are also some methods to change the casing of strings. For example:
~~~
greet.toUpperCase(); // "HELLO, "
greet.toLowerCase(); // "hello, "
~~~