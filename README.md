# What is this?

This is sniff of global method calls Laravel is exposing, that can be replaced with appropriate dependency injection calls, as outlined by article by Frank Prins: https://prinsfrank.nl/2022/09/20/How-to-write-decoupled-unit-tests-in-Laravel

# Usage

Install the extension using Composer:

```
composer require --dev eithed/laravel.dependency-injection-neon
```

Add this to your phpstan.neon:

```
includes:
    - vendor/spaze/phpstan-disallowed-calls/extension.neon
    - vendor/eithed/laravel.dependency-injection-neon/extension.neon
```