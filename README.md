# Python - A guide
This is a document to check everything I learn about Python.
Concepts will be in inverse order of appearance (first concepts I see first go last and vice versa).

## Folders:
-In <code>introduction/</code> you will find different basic programs as to grasp the fundamentals of the language

## 6) Modular Arithmetic

Long division - divide by a number, we get a quotient plus a remainder quotient is integer division <code>//</code>, the remainder is <code>%</code> (Docs)

Problem - get the ones digit of a number
<pre>
<code>num = 49
tens = num // 10
ones = num % 10
print tens, ones
print 10 * tens + ones, num</code>
</pre>

Application - 24 hour clock
<pre>
<code>hour = 20
shift = 8
print (hour + shift) % 24</code>
</pre>


Application - screen wraparound
Spaceship from week seven
<pre>
<code>width = 800
position = 797
move = 5
position = (position + move) % width
print position</code>
</pre>


Data conversion operations

Convert an integer into string - <code>str</code>
Convert an hour into 24-hour format "03:00", always print leading zero
<pre>
<code>hour = 3
ones = hour % 10
tens = hour // 10
print tens, ones, ":00"
print str(tens), str(ones), ":00"
print str(tens) + str(ones) + ":00"</code>
</pre>

## 5) Functions

They need <code>def</code> to define the function, assign some parameters if necessary inside <code>()</code> and end that part of the function, called header, with a <code>:</code>. The rest will be the body and it need indentation to be part of the function body. If it does not have a <code>return</code> statement and it is assigned to a variable, it will return <code>none</code>.

Converts fahrenheit to celsius
<pre>
<code>def fahrenheit2celsius(fahrenheit):
    celsius = (5.0 / 9) * (fahrenheit - 32)
    return celsius</code>
</pre>

Test:
<pre>
<code>c1 = fahrenheit2celsius(32)
c2 = fahrenheit2celsius(212)
print c1, c2</code>
</pre>

Converts fahrenheit to kelvin
<pre>
<code>def fahrenheit2kelvin(fahrenheit):
    celsius = fahrenheit2celsius(fahrenheit)
    kelvin = celsius + 273.15
    return kelvin</code>
</pre>

Test:
<pre>
<code>k1 = fahrenheit2kelvin(32)
k2 = fahrenheit2kelvin(212)
print k1, k2</code>
</pre>

## 4) Variables

There is no variable declaration in Python.
<pre>
<code>my_name = "Joe Warren"</code>
<code>print my_name</code>
</pre>
<pre>
<code>my_age = 51</code>
<code>print my_age</code>
</pre>

<pre>
<code>my_age += 1</code>
<code>print my_age</code>
</pre>

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
+ plus		addition
-	minus		subtraction
*	times		multiplication
/	divided by 	division
** power		exponentiation
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
