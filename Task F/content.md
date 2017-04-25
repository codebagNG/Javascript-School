#Objects And Arrays

## Arrays
Arrays are zero-indexed lists of values. These means they are a collection of the same types of data eg. string. but then there can also be collection of arrays in a single array.

### A simple array example
```
var ArrayExample = [ "hello", "Nigeria" ];
```

### Accessing array items by index
```
var Array2 = [ 'hello' , 'world' , 'foo' , 'bar' ];
console.log( Array2[ 3 ] ) ; // logs ’ bar ’
```

### Testing the size of an array

```
var myarray = [ 'hello', 'surulere' ];
console( myarray.lenght ); // logs 2
```
### Changing the value of an array item
```
var anotherarray = [ "hello", "mushin" ];
anotherarray[1] = 'yaba';
console.log(anotherarray[1]) //logs yaba
```

While it’s possible to change the value of an array item as shown in “Changing the value of an array item”, it’s generally not advised.

### Adding elements to an array

```
var myarray= [ "hello" , "lasu" ];
myarray.push ( "unilag" );
console.log(myarray[2]); //logs unilag
```

#### Working with arrays
var myarray= [ 'l', 'a', 'm', 'i', 'd', 'i' ];
var mystring = myarray.join(''); // logs  'lamidi'

var mysplit = mystring.split(""); // logs  [ 'l', 'a', 'm', 'i', 'd', 'i' ]
```

#Objects

Objects contain one or more key-value pairs. The key portion can be any string. The value portion can be any type of value: a number, a string, an array, a function, or even another object.
[**Definition**: When one of these values is a function, it’s called a method of the object.] Otherwise, they are called properties.

Almost everything in JavaScript is an object — arrays, functions, numbers, even strings. And they all have properties and methods.

### Creating an “object literal”

```
var myObject = {
 greeting : function() {
console.log ( "ekaro, otutuoman, inakwana");
} ,

name : 'chinedu'
};

myobject.greeting(); // logs 'ekaro, otutuoma, inakwana'
console.log( myobject.name ); // logs 'chinedu'
```

Note When creating object literals, you should note that the key portion of each key-value pair can be written as any valid JavaScript identifier, a string (wrapped in quotes) or a number:

```
var m y O b j e c t = {
validIdentifier : 123 ,
'somestring': 456 ,
 99999 : 789
};
```
### Object literals are tottally extremely useful for code organization.