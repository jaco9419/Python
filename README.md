# Python
This is a document to check everything I learn about Python.
Concepts will be in inverse order of appearance (first concepts I see first go last and vice versa).

## 3) Arithmetic Expressions

### int() and float()
<pre>
<code>print type(3), type(3.14159)</code>
<code>print type(3.0)</code>
</pre>
we can convert between data types using int() and float()
note that int() takes the "whole" part of a decimal number and doesn't round
float() applied to integers is boring
<pre>
<code>print int(3.14159), int(-2.8)</code>
<code>print float(3), float(-1)</code>
</pre>

floating point number have around 15 decimal digits of accuracy
pi is 3.1415926535897932384626433832795028841971...
square root of two is 1.4142135623730950488016887242096980785696...


#### arithmetic operators
<pre>
+		plus		addition
-		minus		subtraction
*		times		multiplication
/		divided by 	division
**    power		exponentiation
</pre>

<code>print 1 + 2, 3 - 4, 5 * 6, 2 ** 5</code>

Division in Python 2
If one operand is a decimal (float), the answer is decimal

<code>print 1.0 / 3, 5.0 / 2.0, -7 / 3.0</code>

If both operands are ints, the answer is an int (rounded down)

<code>print 1 / 3, 5 / 2, -7 / 3</code>

expressions - number or a binary operator applied to two expressions
minus is also a unary operator and can be applied to a single expression

</code>print 1 + 2 * 3, 4.0 - 5.0 / 6.0, 7 * 8 + 9 * 10</code>

expressions are entered as sequence of numbers and operations
how are the number and operators grouped to form expressions?
operator precedence - "please excuse my dear aunt sallie" = (), **, *, /, +,-
<pre>
<code>print 1 * 2 + 3 * 4</code>
<code>print 2 + 12</code>
</pre>

always manually group using parentheses when in doubt
<pre>
<code>print 1 * (2 + 3) * 4</code>
<code>print 1 * 5 * 4</code>
</pre>

## 2) print
To print something to the console

## 1) # Comments with a hashtag
To have ignore code for comments
