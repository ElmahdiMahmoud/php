## Syntax

**Tags**

```php
/* Recommended  */
<?php echo 'always available'; ?>

/* Short tag: available since PHP 5.4 */
<? echo 'this is the simplest processing instruction'; ?>

/* ASP tag */
<% echo 'ASP tag style'; %>
```

**Comments**

> PHP supports style comments  'C', 'C++' and shell Unix (style Perl)

```php
// This is a single comment in c++ style

# Another singlw commet line

/ * This is a multiline comment 
another line of comment * /
```

**Outputs**

`echo "Hello World!";` and `print("Hello World!");`

```php
print "print can be used without parentheses.";

echo 'one', 'two', 'three';

echo strftime('%d-%B-%Y, %A');
```

---

### Operators 

The assignment operator
```php
$x = 10;
$x = $x + 15; // $x  = 25

# output
print $x;

# delete $x
unset($x);
```

---

### Variables 

* Variables in PHP start with a  dollar sign `$`
* variable name **must begin** with a letter or underscore 
* Subsequent characters in a variable name can be letters, numbers or symbols underscores in any quantity 
* The variable name is **case sensitive**

```php
$name = "MyName";

<h1><?php echo $name?></h1>
```

* Screening variables
  * $juice = "apple"; 
* What is the result of the following code? 
  * `echo "He drank some $ juice juice.";`
  * `echo "He drank some juice made of $ juices.";` 
* Problem Solving 
  * `echo "He drank some juice made of {$ juice} s.";`
  * `echo "He drank some juice made of $ {juice} s.";`
  
**Access to a character in a string**

Characters in a string can be accessed and modified bydefining them offset of the line starting from beginning
  `$str = 'This is a test.';`
* Get the first character string 
  `$first = $str {0};`
* Get the third character strings 
  `$third = $str {2};`
* Get the last character string 
  `$last = $str {strlen ($str) -1};`
* Change the last character of a string 
  `$str {strlen ($str) -1} = '!';`
---


### Constants 

* Constants can be determined by using the define (), and not assigning values 
  * `define ("CONSTANT", "Hello world."); `
  * `const CONSTANT = "Hello World."; // PHP 5.3 `
* Constants do not have a dollar sign ($) 
  * `echo CONSTANT; // Outputs "Hello, world." `
* Constants may be defined and accessed anywhere without accounting scope 
* Constants may not be redefined or undefined once initial announcement 
* Constants may only evaluate to scalar values 
* Declare constant insensitive 
  * `define ("CONSTANT", "Hello World.", True);`

---


### Types 

PHP - dynamically typed language (loosely typed) 

* PHP supports eight primitive types 
* Four scalar types: 
  1. boolean 
  2. integer 
  3. float (floating point number) 
  4. string 
* Two compound types: 
  1. array 
  2. object 
* Two special types: 
  1. resource 
  2. NULL

##### Type: boolean

* This is the simplest type
* expresses a truth value: `TRUE` or `FALSE` 
* Keywords TRUE and FALSE are case independent 
* Assign **$foo** the value **TRUE**
  * `$foo = True;`

##### Type: integer and floats

Integer
```php
    $i = 1234; // Decimal number
    $i = -123; // A negative number 
    $i = 0123; // 83 octal 
    $i = 0x1A; // 26 hex 
    $i = 0b101; // Binary 5 (PHP 5.4) 
```

Float
```php
   $f = 1.234; 
   $f = 1.2e3; // 1200 
   $f = 7E-10; // 0.0000000007
```

##### Type: string (double quotes)

* If the string is specified in double quotes, variables parsed within it 
  * `$juice = "apple";` 
* Outputs: He drank some apple juice 
  * `echo "He drank some $ juice juice.";` 
* Outputs: There will be a newline 
  * `echo "There will be translated into \ n new line.";` 
* Outputs: screening "inside" double quotes 
  * `echo "screening \" in \ "double quotes.";`
  

##### Type: string (single quotes)

* In contrast to the double-quote syntax, variables, and escape sequences for special characters enclosed in single quotes, not processed 
  * `$juice = "apple";` 
* Outputs: He drank some $ juice juice 
  * echo 'He drank some $ juice juice.'; 
* Outputs: There will be translated into \ n new line 
  * echo 'Here is a translation from a \ n new line.'; 
* Outputs: screening 'inside' single quotes 
  * echo 'screening \' in \ 'single quotes.';
  

##### Type: string (heredoc)
```php
echo <<< LABEL
My name is "$ name". Newline .
Before the line is worth a tab character.
This should print a capital 'A': \ x41
LABEL;
```
* The identifier must contain only alphanumeric characters and underscores, and must start with a digit ( sign underscore allowed )
* After `<<<` operator , an identifier , and then only line feed
* The closing identifier **must** be in the first column of the line
* line with the closing identifier **must** not contain other characters, except possibly a semicolon (`;`)
  

##### Type: string (NULL)
The special NULL value represents variable without values​ 
* NULL - the only possible value of type NULL 
* A variable is **null**, if: 
  * it has been assigned the constant `NULL`
  * it has not been assigned any value 
  * it was removed by the `unset ()`
* `$ var = NULL;`

---


### Control structures 

If the string is enclosed in double quotes, PHP recognizes escape sequences for special characters: 
* `\n` linefeed (LF or 0x0A (10) in ASCII) 
* `\r` carriage return (CR or 0x0D (13) in ASCII) 
* `\t` horizontal tab (HT or 0x09 (9) in ASCII) 
* `\\` backslash 
* `\$` dollar sign 
* `\"` double quote
