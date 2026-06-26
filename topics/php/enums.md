# PHP Enums (PHP 8.1+)

## Basic Enum (Pure)
```php
enum Status
{
    case Active;
    case Inactive;
    case Pending;
}

$status = Status::Active;
```

## Backed Enum (string or int)
```php
enum AlertType: string
{
    case BalanceAbove = 'balance_above';
    case BalanceBelow = 'balance_below';
}

// Get value
AlertType::BalanceAbove->value; // 'balance_above'

// From value
AlertType::from('balance_above'); // AlertType::BalanceAbove
AlertType::tryFrom('unknown');    // null (no exception)
```

## Enum methods
```php
enum Status: string
{
    case Active = 'active';
    case Inactive = 'inactive';

    public function label(): string
    {
        return match($this) {
            Status::Active => 'Active user',
            Status::Inactive => 'Inactive user',
        };
    }
}
```

## Enum in Doctrine (Symfony)
```php
#[ORM\Column(enumType: AlertType::class)]
private AlertType $type;
```

## Key points
- Pure enums have no value
- Backed enums have string or int value
- `from()` throws exception if value not found
- `tryFrom()` returns null if value not found
- Enums can implement interfaces
- Enums can have methods and constants
- Enums cannot be instantiated with `new`