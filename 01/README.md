## Syntax

### Tags

```php
/* Recommended  */
<?php echo 'always available'; ?>

/* Short tag: available since PHP 5.4 */
<? echo 'this is the simplest processing instruction'; ?>

/* ASP tag */
<% echo 'ASP tag style'; %>
```

### Comments

> PHP supports style comments  'C', 'C++' and shell Unix (style Perl)

```php
// This is a single comment in c++ style

# Another singlw commet line

/ * This is a multiline comment 
another line of comment * /
```

### Outputs

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


---


### Constants 

---


### Types 

PHP - dynamically typed language (loosely typed) 

* PHP supports eight primitive types 
  * Four scalar types: 
    * boolean 
    * integer 
    * float (floating point number) 
    * string 
* Two compound types: 
  * array 
  * object 
* Two special types: 
  * resource 
  * NULL

##### Type: boolean

* This is the simplest type
* expresses a truth value: `TRUE` or `FALSE` 
* Keywords TRUE and FALSE are case independent 
* Assign **$foo** the value **TRUE**
  * `$foo = True;`

##### Type: integer and floats

* Integer 
```php
    $i = 1234; // Decimal number
    $i = -123; // A negative number 
    $i = 0123; // 83 octal 
    $i = 0x1A; // 26 hex 
    $i = 0b101; // Binary 5 (PHP 5.4) 
```
* Float 
```php
   $f = 1.234; 
   $f = 1.2e3; // 1200 
   $f = 7E-10; // 0.0000000007
```
---


### Control structures 

