# Loops
Loops let you run a block of code a certain number of times.

```
// logs ’ try 0 ’ , ’ try 1 ’ , ... , ’ try 4 ’
for ( var i =0; i <5; i ++) {
c o n s o l e . log ( ’ try ’ + i );
}
```

Note that in Loops even though we use the keyword var before the variable name i, this does not “scope” the variable
i to the loop block.

### The for loop

A for loop is made up of four statements and has the following structure:

```
for ([ i n i t i a l i s a t i o n ]; [ c o n d i t i o n a l ]; [ i t e r a t i o n ])
[ l o o p B o d y ]
```

The initialisation statement is executed only once, before the loop starts. It gives you an opportunity to prepare or declare any variables. The conditional statement is executed before each iteration, and its return value decides whether or not the loop is to continue. If the conditional statement evaluates to a falsey value then the loop stops. The iteration statement is executed at the end of each iteration and gives you an opportunity to change
the state of important variables. Typically, this will involve incrementing or decrementing a counter and thus bringing the loop ever closer to its end. The loopBody statement is what runs on every iteration. It can contain anything you want. You’ll typically
have multiple statements that need to be executed and so will wrap them in a block ( {...}). Here’s a typical for loop:


```
for ( var i = 0 , li m i t = 100; i < li m i t ; i ++) {
// This b l o c k will be e x e c u t e d 100 t i m e s
c o n s o l e . log ( ’ C u r r e n t l y at ’ + i );
// Note : the last log will be ” C u r r e n t l y at 99 ”
}
```

### The while loop

A while loop is similar to an if statement, except that its body will keep executing until the condition
evaluates to false.

```
w h i l e ([ c o n d i t i o n a l ]) [ l o o p B o d y ]
```
Here’s a typical while loop:

```
var i = 0;
w h i l e ( i < 100) {
// This b l o c k will be e x e c u t e d 100 t i m e s
c o n s o l e . log ( ’ C u r r e n t l y at ’ + i );
i ++; // i n c r e m e n t i
}
```

You’ll notice that we’re having to increment the counter within the loop’s body. It is possible to combine the conditional and incrementer, like so:

```
var i = -1;
w h i l e (++ i < 100) {
// This b l o c k will be e x e c u t e d 100 t i m e s
c o n s o l e . log ( ’ C u r r e n t l y at ’ + i );
}
```
Notice that we’re starting at -1 and using the prefix incrementer (++i).

### The do-while loop

This is almost exactly the same as the while loop, except for the fact that the loop’s body is executed at least once before the condition is tested.

```
do [ l o o p B o d y ] w h i l e ([ c o n d i t i o n a l ])
```
Here’s a do-while loop:

```
do {
// Even t h o u g h the c o n d i t i o n e v a l u a t e s to f a l s e
// this loop ’ s body will s t i l l e x e c u t e once .
a l e r t ( ’ Hi t h e r e ! ’);
} w h i l e ( f a l s e );
```

These types of loops are quite rare since only few situations require a loop that blindly executes at least
once. Regardless, it’s good to be aware of it.


### Breaking and continuing

Usually, a loop’s termination will result from the conditional statement not evaluating to true, but it is possible to stop a loop in its tracks from within the loop’s body with the break statement.

```
for ( var i = 0; i < 10; i ++) {
if ( s o m e t h i n g ) {
b r e a k ;
}
}
```

You may also want to continue the loop without executing more of the loop’s body. This is done using the continue statement.

```
for ( var i = 0; i < 10; i ++) {
if ( s o m e t h i n g ) {
c o n t i n u e ;
}
// The f o l l o w i n g s t a t e m e n t will only be e x e c u t e d
// if the c o n d i t i o n a l ’ something ’ has not been met
c o n s o l e . log ( ’ I have been reached ’);
}
```