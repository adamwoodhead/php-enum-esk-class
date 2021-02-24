
# php-enums

### To Be Replaced
This helper class will be obsolete from PHP 8.1, see https://wiki.php.net/rfc/enumerations

### Example of a typical enum:

```php
class DayOfWeek extends Enum
{
    const Sunday    = 0;
    const Monday    = 1;
    const Tuesday   = 2;
    const Wednesday = 3;
    const Thursday  = 4;
    const Friday    = 5;
    const Saturday  = 6;
}
```

## Usage examples:

```
$monday = DayOfWeek::Monday
DayOfWeek::isValidName('Monday')
DayOfWeek::isValidName('monday', $strict = true)
DayOfWeek::isValidValue(0)
DayOfWeek::fromString('Monday')
DayOfWeek::toString(DayOfWeek::Tuesday)
DayOfWeek::toString(5)
```
```
(int) 1
(bool) true
(bool) false
(bool) true
(int) 1
(string) "Tuesday"
(string) "Friday"
```

### Credit
- https://stackoverflow.com/a/40658901
