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

---


### Control structures 

