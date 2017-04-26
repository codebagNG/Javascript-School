# Loops
Loops let you run a block of code a certain number of times.

```
// it outputs try 5 times
for ( var i =0; i <5; i ++) {
console.log ( ’ try ’ + i );
}
```

Note that in Loops even though we use the keyword var before the variable name i, this does not “scope” the variable
i to the loop block. Scope is a concept of having variables under a block of code, and that variables only works for that block. there is general scoping too, its when the variable isnt under any block of code(function, a loop block or something else)

### The for loop

A for loop is made up of four statements and has the following structure:

```
for ([ initialisation ]; [ conditional ]; [ value to iterate over ])
[then the loop contents]
```

The initialisation statement is executed only once, before the loop starts. The conditional statement is executed before each iteration value, and its return value decides whether or not the loop is to continue. If the conditional statement evaluates to a falsey value then the loop stops. The iteration statement is executed at the end of each iteration and gives you an opportunity to change the state of important variables. Here’s a typical for loop:


```
for ( var i = 0 , limit = 50; i < limit ; i++) {
// the block executes 50 times
console.log ( "this is the prsent number" + i );
}
```

### The while loop

A while loop is similar to an if statement, except that its body will keep executing until the condition evaluates to false.

```
while([conditional]) [loop content]
```
Here’s a typical while loop:

```
var i = 0;
while( i < 100) {
// This block executes 20 times
	console.log( "the present number is" + i );
	i++; // this statement is the increment
}
```

You’ll notice that we’re having to increment the counter within the loop’s body. It is possible to combine the conditional and incrementer, like so:

```
var i = -1;
while(++i < 100) {
console.log( "the present number is" + i );
}
```
Notice that we’re starting at -1 and using the prefix incrementer (++i).

### The do-while loop

This is almost exactly the same as the while loop, except for the fact that the loop’s body is executed at least once before the condition is started.

```
do [ Loopbody ]
while([ conditional ])
```
Here’s a do-while loop:

```
do {
// notice that the code executes once even though the conditional is false
alert( " Audu loves chidinma!! ");
}
while( false );
```

These loops are not very common and are hardly used 

### Breaking and continuing

A loop stops when the condition over it is fulfilled. But there are cases you might want the loop to stop before then. thats where breaking and continuing does  


```
for ( var i = 0; i < 10; i ++) {
if ( condition) {
 break;
}
}
```
This second case implements the continue statement.

```
for ( var i = 0; i < 10; i ++) {
if (condition) {
continue ;
}
//the code only executes after the condition has been met
}
```