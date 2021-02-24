
# php-enums

### Implements the abstract base for all enum types
- http://stackoverflow.com/a/2324746/1003020
- http://stackoverflow.com/a/254543/1003020

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
