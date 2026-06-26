# PHP Attributes

## What are attributes?
Metadata added to classes, methods, properties or parameters using the `#[...]` syntax (PHP 8.0+).
Replaces docblock annotations (@ORM\Entity, @Route, etc.).

## Syntax
```php
#[Attribute]
class MyAttribute
{
    public function __construct(public string $value) {}
}

#[MyAttribute('hello')]
class MyClass {}
```

## Usage in Symfony
- `#[Route]` — define routes on controllers
- `#[ORM\Entity]` — Doctrine entity mapping
- `#[AsMessageHandler]` — declare a Messenger handler
- `#[AsSchedule]` — declare a Scheduler
- `#[AsCommand]` — declare a Console command