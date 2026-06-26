# PHP Interfaces

## What is an Interface?
A contract that classes must implement. Defines method signatures without implementation.

## Basic syntax
```php
interface PaymentGatewayInterface
{
    public function charge(float $amount): bool;
    public function refund(float $amount): bool;
}

class StripeGateway implements PaymentGatewayInterface
{
    public function charge(float $amount): bool
    {
        return true;
    }

    public function refund(float $amount): bool
    {
        return true;
    }
}
```

## Multiple interfaces
```php
interface Serializable
{
    public function serialize(): string;
}

interface Loggable
{
    public function log(): void;
}

class Order implements Serializable, Loggable
{
    public function serialize(): string { return json_encode($this); }
    public function log(): void { echo 'logged'; }
}
```

## Interface extending interface
```php
interface ReadableInterface
{
    public function read(): string;
}

interface WritableInterface extends ReadableInterface
{
    public function write(string $data): void;
}
```

## Real Symfony examples
```php
class User implements UserInterface, PasswordAuthenticatedUserInterface {}

class AddressVoter extends Voter {}

class AddressSyncSchedule implements ScheduleProviderInterface {}
```

## Key points
- Interfaces cannot have properties
- All methods are public and abstract by default
- A class can implement multiple interfaces
- Interfaces can extend multiple interfaces
- Constants are allowed in interfaces
- Type-hinting against interfaces enables loose coupling