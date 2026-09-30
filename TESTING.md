# Testing Guidelines

## Unit Tests

```bash
php artisan test
```

## Feature Tests

```bash
php artisan test --filter=Feature
```

## Test Coverage

Ensure all controllers and models have corresponding tests.

## Creating Tests

```bash
php artisan make:test FeatureTest
php artisan make:test UnitTest --unit
```

## CI/CD Integration

Tests run automatically on push via GitHub Actions.
