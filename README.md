php-date-prefix
===============

PHP [subsidizes the very worst programmers](http://news.php.net/php.internals/67458) by triggering pointless timezone `E_WARNINGS` for something
that isn't a real error. This inanity makes effective unit-testing difficult and promotes poor design
practices. But now, thankfully, you can use `php-date-prefix` to solve all your problems! No more
requiring a moronic php.ini file just to use PHP as a programming language!

### Usage:

```php
<?php
require 'php-date-prefix.php'; // problem solved!
echo date('Y-m-d'),  " doesn't trigger errors! Woohoo!\n";
```

### Source Code:

```php
<?php
// Derick Rethans hates good design.
date_default_timezone_set('UTC');
```

##### Epilogue:

Mr. Rethans has done *a lot of great work* for PHP. This is not meant to antagonize ... just to point out a glaring language-level PHP fail.
