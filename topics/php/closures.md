# PHP Closures & Anonymous Functions

## Anonymous function
```php
$greet = function(string $name): string {
    return "Hello $name";
};

$greet('Florent');
```

## Arrow function (PHP 7.4+)
```php
$multiplier = 3;
$multiply = fn(int $n) => $n * $multiplier;

$multiply(5);
```

## Difference: anonymous function vs arrow function
```php
$value = 10;

$fn1 = function() use ($value) {
    return $value * 2;
};

$fn2 = fn() => $value * 2;
```

## Real examples from your projects
```php
return $this->json(array_map(static fn(WatchedAddress $a) => [
    'id' => $a->getId(),
    'address' => $a->getAddress(),
], $addresses));

return array_values(array_map(fn(array $tx) => [
    'txid' => $tx['txid'],
    'confirmed' => $tx['status']['confirmed'] ?? false,
], $transactions));
```

## Closures as callbacks
```php
$numbers = [1, 2, 3, 4, 5];

$doubled = array_map(fn(int $n) => $n * 2, $numbers);

$even = array_filter($numbers, fn(int $n) => $n % 2 === 0);

$sum = array_reduce($numbers, fn(int $carry, int $n) => $carry + $n, 0);
```

## Key points
- Anonymous functions must use `use` to capture outer variables
- Arrow functions auto-capture outer scope (read-only)
- Arrow functions are single-expression only
- Closures are instances of the `Closure` class
- `static` keyword prevents binding to `$this`