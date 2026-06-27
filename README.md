# Symfony 8 Certification Preparation

Personal cheat sheets and key points for the Symfony 8 SensioLabs certification.

**Exam:** 75 questions / 15 topics / 90 minutes / In English

---

## Topics

### 1. PHP
| Sub-topic | Documentation |
|-----------|--------------|
| PHP API up to PHP 8.4 | https://www.php.net/manual/en/ |
| Object Oriented Programming | https://www.php.net/manual/en/language.oop5.php |
| Attributes | https://www.php.net/manual/en/language.attributes.php |
| Interfaces | https://www.php.net/manual/en/language.oop5.interfaces.php |
| Anonymous functions and closures | https://www.php.net/manual/en/functions.anonymous.php |
| Abstract classes | https://www.php.net/manual/en/language.oop5.abstract.php |
| Exception and error handling | https://www.php.net/manual/en/language.exceptions.php |
| Traits | https://www.php.net/manual/en/language.oop5.traits.php |
| Enums | https://www.php.net/manual/en/language.enumerations.php |

### 2. HTTP
| Sub-topic | Documentation |
|-----------|--------------|
| HTTP Specification (RFC 9110) | https://httpwg.org/specs/rfc9110.html |
| Status codes | https://httpwg.org/specs/rfc9110.html#status.codes |
| HTTP request | https://symfony.com/doc/8.0/components/http_foundation.html |
| HTTP response | https://symfony.com/doc/8.0/components/http_foundation.html |
| HTTP methods | https://httpwg.org/specs/rfc9110.html#methods |
| Cookies | https://symfony.com/doc/8.0/components/http_foundation.html |
| Caching | https://symfony.com/doc/8.0/http_cache.html |
| Content negotiation | https://httpwg.org/specs/rfc9110.html#content.negotiation |
| Language detection | https://symfony.com/doc/8.0/translation.html |
| Symfony HttpClient | https://symfony.com/doc/8.0/http_client.html |

### 3. Symfony Architecture
| Sub-topic | Documentation |
|-----------|--------------|
| HttpFoundation component | https://symfony.com/doc/8.0/components/http_foundation.html |
| Symfony Flex | https://symfony.com/doc/8.0/setup/flex.html |
| Components and Bridges | https://symfony.com/doc/8.0/components/index.html |
| Code organization | https://symfony.com/doc/8.0/best_practices.html |
| Request handling | https://symfony.com/doc/8.0/components/http_kernel.html |
| Exception handling | https://symfony.com/doc/8.0/controller/error_pages.html |
| Event dispatcher and kernel events | https://symfony.com/doc/8.0/event_dispatcher.html |
| Official best practices | https://symfony.com/doc/8.0/best_practices.html |
| Backward compatibility promise | https://symfony.com/doc/8.0/contributing/code/bc.html |
| Naming conventions | https://symfony.com/doc/8.0/contributing/code/standards.html |

### 4. Controllers
| Sub-topic | Documentation |
|-----------|--------------|
| HttpKernel component | https://symfony.com/doc/8.0/components/http_kernel.html |
| The base AbstractController class | https://symfony.com/doc/8.0/controller.html |
| The request | https://symfony.com/doc/8.0/components/http_foundation.html |
| The response | https://symfony.com/doc/8.0/components/http_foundation.html |
| The session | https://symfony.com/doc/8.0/session.html |
| The flash messages | https://symfony.com/doc/8.0/controller.html |
| HTTP redirects | https://symfony.com/doc/8.0/controller.html |
| File upload | https://symfony.com/doc/8.0/controller/upload_file.html |
| Argument value resolvers | https://symfony.com/doc/8.0/controller/value_resolver.html |

### 5. Routing
| Sub-topic | Documentation |
|-----------|--------------|
| Routing component | https://symfony.com/doc/8.0/routing.html |
| Configuration (YAML and PHP attributes) | https://symfony.com/doc/8.0/routing.html |
| Restrict URL parameters | https://symfony.com/doc/8.0/routing.html |
| Set default values to URL parameters | https://symfony.com/doc/8.0/routing.html |
| URLs generation | https://symfony.com/doc/8.0/routing.html |
| Special internal routing attributes | https://symfony.com/doc/8.0/routing.html |
| Domain name matching | https://symfony.com/doc/8.0/routing.html |
| HTTP methods matching | https://symfony.com/doc/8.0/routing.html |
| Router debugging | https://symfony.com/doc/8.0/routing.html |

### 6. Templating with Twig
| Sub-topic | Documentation |
|-----------|--------------|
| TwigBundle | https://symfony.com/doc/8.0/templates.html |
| Twig syntax | https://twig.symfony.com/doc/3.x/ |
| Template inheritance | https://symfony.com/doc/8.0/templates.html |
| Filters and functions | https://twig.symfony.com/doc/3.x/filters/index.html |
| URLs generation | https://symfony.com/doc/8.0/templates.html |
| Translations | https://symfony.com/doc/8.0/translation.html |
| Debugging variables | https://symfony.com/doc/8.0/templates.html |

### 7. Forms
| Sub-topic | Documentation |
|-----------|--------------|
| Form component | https://symfony.com/doc/8.0/forms.html |
| Forms creation | https://symfony.com/doc/8.0/forms.html |
| Form types | https://symfony.com/doc/8.0/reference/forms/types.html |
| CSRF protection | https://symfony.com/doc/8.0/security/csrf.html |
| Data transformers | https://symfony.com/doc/8.0/form/data_transformers.html |
| Form events | https://symfony.com/doc/8.0/form/events.html |
| Form type extensions | https://symfony.com/doc/8.0/form/create_form_type_extension.html |

### 8. Data Validation
| Sub-topic | Documentation |
|-----------|--------------|
| Validator component | https://symfony.com/doc/8.0/validation.html |
| Built-in validation constraints | https://symfony.com/doc/8.0/reference/constraints.html |
| Validation groups | https://symfony.com/doc/8.0/validation/groups.html |
| Custom callback validators | https://symfony.com/doc/8.0/reference/constraints/Callback.html |

### 9. Dependency Injection
| Sub-topic | Documentation |
|-----------|--------------|
| Service container | https://symfony.com/doc/8.0/service_container.html |
| Services autowiring | https://symfony.com/doc/8.0/service_container/autowiring.html |
| Service decoration | https://symfony.com/doc/8.0/service_container/service_decoration.html |
| Tags | https://symfony.com/doc/8.0/service_container/tags.html |
| Compiler passes | https://symfony.com/doc/8.0/service_container/compiler_passes.html |
| Service locators | https://symfony.com/doc/8.0/service_container/service_subscribers_locators.html |

### 10. Security
| Sub-topic | Documentation |
|-----------|--------------|
| Authentication | https://symfony.com/doc/8.0/security.html |
| Authorization | https://symfony.com/doc/8.0/security.html#access-control-authorization |
| Firewalls | https://symfony.com/doc/8.0/security.html |
| Voters and voting strategies | https://symfony.com/doc/8.0/security/voters.html |
| Password hashers | https://symfony.com/doc/8.0/security/passwords.html |

### 11. Messenger
| Sub-topic | Documentation |
|-----------|--------------|
| Messenger component | https://symfony.com/doc/8.0/messenger.html |
| Transports | https://symfony.com/doc/8.0/messenger.html |
| Messages and handlers | https://symfony.com/doc/8.0/messenger.html |
| Workers | https://symfony.com/doc/8.0/messenger.html |
| Middleware | https://symfony.com/doc/8.0/messenger/middleware.html |

### 12. Console
| Sub-topic | Documentation |
|-----------|--------------|
| Console component | https://symfony.com/doc/8.0/console.html |
| Custom commands | https://symfony.com/doc/8.0/console.html |
| Options and arguments | https://symfony.com/doc/8.0/console/input.html |
| Console events | https://symfony.com/doc/8.0/components/console/events.html |

### 13. Automated Tests
| Sub-topic | Documentation |
|-----------|--------------|
| Unit tests with PHPUnit | https://symfony.com/doc/8.0/testing.html |
| Functional tests with PHPUnit | https://symfony.com/doc/8.0/testing.html |
| Client object | https://symfony.com/doc/8.0/testing.html |
| Crawler object | https://symfony.com/doc/8.0/testing.html |

### 14. Miscellaneous
| Sub-topic | Documentation |
|-----------|--------------|
| Configuration | https://symfony.com/doc/8.0/configuration.html |
| Error handling | https://symfony.com/doc/8.0/controller/error_pages.html |
| Web Profiler | https://symfony.com/doc/8.0/profiler.html |
| HTTP Caching | https://symfony.com/doc/8.0/http_cache.html |
| Cache component | https://symfony.com/doc/8.0/cache.html |
| Mailer component | https://symfony.com/doc/8.0/mailer.html |
| Serializer component | https://symfony.com/doc/8.0/serializer.html |
| EventDispatcher component | https://symfony.com/doc/8.0/event_dispatcher.html |