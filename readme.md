# Project Title

This project is a **Laravel application** created to **experiment with Unit Testing using PEST v4**.

The main goal of this project is to understand PEST v4 syntax, structure, and best practices for writing clean and readable unit tests.

## Requirements

* PHP >= 8.2
* Composer
* Laravel (according to the project version)
* PEST v4

## Installation

Clone the repository and install dependencies:
git clone <git@github.com:MinKhantMaw/pest-test-v4.git>
cd pest-test-v4

```bash
composer install
cp .env.example .env
php artisan key:generate
```

If the project uses a database, update your `.env` file with the correct database credentials and run migrations:

```bash
php artisan migrate
```

## Testing Setup (PEST v4)

PEST v4 is already configured in this project.

* Unit tests are located in the `tests/Unit` directory
* Feature tests are located in the `tests/Feature` directory
* The project uses PEST's expressive syntax such as `it()`, `describe()`, and `expect()`

### Example Test

```php
it('can add two numbers', function () {
    expect(1 + 1)->toBe(2);
});
```

## Running Tests

Run all tests using:

```bash
php artisan test
# or
./vendor/bin/pest
```

Run a specific test file:

```bash
./vendor/bin/pest tests/Unit/ExampleTest.php
```

## Notes

* This project uses **PEST v4 simplified syntax** for better readability
* Unit tests focus on testing core business logic in isolation
* Suitable for learning and experimenting with modern Laravel testing practices

## References

* [https://pestphp.com](https://pestphp.com)

---

Developed for learning and testing purposes 🚀
