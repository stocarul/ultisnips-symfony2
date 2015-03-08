# PHPUnit snippets for vim #

All shortcuts start with the `pu` prefix and are both short and intuitive:

### Classes ###

`putest`

```php
<?php

namespace AlgoTech\MainBundle\Tests;

class CustomTest extends \PHPUnit_Framework_TestCase
{

}
```

### Mockings ###

`pumock`

```php
$this
    ->getMockBuilder('Class')
    ->setMethods(array())
    ->disableOriginalConstructor()
    ->getMock()
```

`pumockp`

```php
$this
    ->getMockBuilder('Class')
    ->setConstructorArgs(array())
    ->setMethods(array())
    ->getMock()
```

### Expectations ###

`puexpects`

```php
->expects($this->once())
->method('method')
->with($this->equalTo('something'))
->will($this->returnValue(null))
```

`puexpectsat`

```php
->expects($this->at(0))
->method('method')
->with($this->equalTo('something'))
->will($this->returnValue(true))
```