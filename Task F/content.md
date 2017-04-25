#Objects And Arrays

## Arrays
Arrays are zero-indexed lists of values. They are a handy way to store a set of related items of the same type (such as strings), though in reality, an array can include multiple types of items, including other arrays.

### A simple array
```
var m y A r r a y = [ ’ hello ’ , ’ world ’ ];
Accessing array items by index
var m y A r r a y = [ ’ hello ’ , ’ world ’ , ’ foo ’ , ’ bar ’ ];
c o n s o l e . log ( m y A r r a y [ 3 ] ) ; // logs ’ bar ’
Testing the size of an array
var m y A r r a y = [ ’ hello ’ , ’ world ’ ];
c o n s o l e . log ( m y A r r a y . l e n g t h ); // logs 2
Changing the value of an array item
var m y A r r a y = [ ’ hello ’ , ’ world ’ ];
m y A r r a y [1] = ’ changed ’;
```

While it’s possible to change the value of an array item as shown in “Changing the value of an array item”, it’s generally not advised.

### Adding elements to an array

```
var m y A r r a y = [ ’ hello ’ , ’ world ’ ];
m y A r r a y . push ( ’ new ’);
Working with arrays
var m y A r r a y = [ ’h ’ , ’e ’ , ’l ’ , ’l ’ , ’o ’ ];
var m y S t r i n g = m y A r r a y . join ( ’ ’); // ’ hello ’
var m y S p l i t = m y S t r i n g . s p l i t ( ’ ’); // [ ’h ’ , ’e ’ , ’l ’ , ’l ’ , ’o ’ ]
```

#Objects

Objects contain one or more key-value pairs. The key portion can be any string. The value portion can be any type of value: a number, a string, an array, a function, or even another object.
[Definition: When one of these values is a function, it’s called a method of the object.] Otherwise, they are called properties.

As it turns out, nearly everything in JavaScript is an object — arrays, functions, numbers, even strings —
and they all have properties and methods.

###Creating an “object literal”

```
var m y O b j e c t = {
s a y H e l l o : f u n c t i o n () {
c o n s o l e . log ( ’ hello ’);
} ,
m y N a m e : ’ Rebecca ’
};
m y O b j e c t . s a y H e l l o (); // logs ’ hello ’
c o n s o l e . log ( m y O b j e c t . m y N a m e ); // logs ’ Rebecca ’
```

Note When creating object literals, you should note that the key portion of each key-value pair can be written as any valid JavaScript identifier, a string (wrapped in quotes) or a number:

```
var m y O b j e c t = {
v a l i d I d e n t i f i e r : 123 ,
’ some string ’: 456 ,
9 9 9 9 9 : 789
};
```
Object literals can be extremely useful for code organization.