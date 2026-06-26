# PHP Traits

## What is a Trait?
A mechanism for code reuse in single inheritance languages.
A trait cannot be instantiated on its own.

## Basic syntax
```php
trait Timestampable
{
    private \DateTimeImmutable $createdAt;

    public function getCreatedAt(): \DateTimeImmutable
    {
        return $this->createdAt;
    }

    public function initTimestamps(): void
    {
        $this->createdAt = new \DateTimeImmutable();
    }
}

class User
{
    use Timestampable;
}

$user = new User();
$user->initTimestamps();
$user->getCreatedAt();
```

## Multiple traits
```php
class User
{
    use Timestampable, SoftDeletable, Loggable;
}
```

## Conflict resolution
```php
class MyClass
{
    use TraitA, TraitB {
        TraitA::hello insteadof TraitB;
        TraitB::hello as helloFromB;
    }
}
```

## Real Symfony example
```php
trait DatabasePrimer
{
    protected function resetDatabase(KernelBrowser $client): void
    {
        $em = $client->getContainer()->get(EntityManagerInterface::class);
        $schemaTool = new SchemaTool($em);
        $metadata = $em->getMetadataFactory()->getAllMetadata();
        $schemaTool->dropSchema($metadata);
        $schemaTool->createSchema($metadata);
    }
}
```

## Key points
- Traits solve the single inheritance limitation
- A class can use multiple traits
- Traits can have properties, methods and abstract methods
- Traits cannot implement interfaces directly
- Conflicts between traits must be resolved explicitly