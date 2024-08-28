## Variables

**Definition**: Variables are used to store data that can be referenced and manipulated throughout a script.

**Syntax**:
```php
$variableName = value;
$name = "John";       // String
$age = 30;            // Integer
$price = 19.99;       // Float
$isValid = true;      // Boolean
```

## Data Types 

**Definition**: PHP supports several data types, including strings, integers, floats, Booleans, arrays, and objects.

**Examples**: 

```php
$string = "Hello, World!";   // String
$integer = 42;               // Integer
$float = 3.14;               // Float
$boolean = false;            // Boolean

// Array
$array = [1, 2, 3, 4];

// Object
class Person {
    public $name;
    public $age;
}

$person = new Person();
$person->name = "Alice";
$person->age = 25;
```

## Operators

**Definition**: Operators are symbols used to perform operations on variables and values.

**Types**:

- **Arithmetic Operators**: 
```PHP
$sum = 5 + 3;        // Addition
$difference = 5 - 3; // Subtraction
$product = 5 * 3;    // Multiplication
$quotient = 5 / 3;   // Division
$modulus = 5 % 3;    // Modulus
```

- Comparison Operators
```php
$isEqual = (5 == 3);      // Equal to
$isIdentical = (5 === 3); // Identical to
$isNotEqual = (5 != 3);   // Not equal to
$isGreater = (5 > 3);     // Greater than
$isLess = (5 < 3);        // Less than
```

- **Logical Operators**:
```php
$and = (true && false);   // Logical AND
$or = (true || false);    // Logical OR
$not = !true;             // Logical NOT
```

- **Assignment Operators**:
```php
$a = 5;       // Assignment
$a += 3;      // Addition assignment
$a -= 3;      // Subtraction assignment
$a *= 3;      // Multiplication assignment
$a /= 3;      // Division assignment
```

## Control Structures

**Definition**: Control structures are used to control the flow of execution in a script.

- **If Statement**:
```php
if ($condition) {
    // code to execute if condition is true
} elseif ($anotherCondition) {
    // code to execute if anotherCondition is true
} else {
    // code to execute if all conditions are false
}
```

- **Switch Statement**:
```php
switch ($variable) {
    case 'value1':
        // code to execute if $variable == 'value1'
        break;
    case 'value2':
        // code to execute if $variable == 'value2'
        break;
    default:
        // code to execute if no case matches
}
```

## Loops

 - **For Loop**:
 ```php
 for ($i = 0; $i < 10; $i++) {
    // code to execute
}```

 - **While Loop**:
 ```php
 while ($condition) {
    // code to execute
}
```
 
 - **Do-While Loop**:
 ```php
 do {
    // code to execute
} while ($condition);
```

## Functions and Error Handling

**Definition**: Functions encapsulate code into reusable blocks. Error handling manages errors that occur during script execution.

- **Function Definition and Call**:
```php
function myFunction($param) {
    // code to execute
    return $result;
}

$result = myFunction('argument');
```

### *Error Handling:

- **Try-Catch Block**:
```php
try {
    // code that may throw an exception
} catch (Exception $e) {
    // code to execute if an exception occurs
    echo 'Caught exception: ',  $e->getMessage(), "\n";
}
```

 - **Custom Error Handling**:
 ```php
 function customError($errno, $errstr) {
    echo "Error [$errno]: $errstr";
}

set_error_handler("customError");
```

