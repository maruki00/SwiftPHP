
# SwiftPHP

**SwiftPHP** is a fast, lightweight, and clean PHP framework built for modern application development using **Domain-Driven Design (DDD)** principles.

> **Swift** development, **strong** architecture.

---

## ✨ Features

- Lightweight and high performance
- Clean Domain-Driven Design (DDD) structure
- Minimalistic and extendable core
- Core framework located at `vendor/core`
- Easy to learn, easy to contribute

---

## 🏛️ Architecture

SwiftPHP is based on **Domain-Driven Design (DDD)** concepts. The project structure separates the main responsibilities into clear layers:

- **Domain Layer**: Business rules (Entities, Value Objects, Repositories)
- **Application Layer**: Application services, use cases
- **Infrastructure Layer**: Database, file system, external services
- **Presentation Layer**: Controllers, Views, API handlers

The **core** logic of the framework is isolated under:

```
vendor/core/
```

This ensures the core remains reusable, stable, and independent of business logic.

---

## 📂 Project Structure

```
/app
    /Domain
    /Application
    /Infrastructure
    /Presentation
/public
    index.php
/routes
    web.php
/vendor
    /core  --> (SwiftPHP Core Framework)
/composer.json
/README.md
```

---

## 🚀 Getting Started

1. Clone SwiftPHP:

```bash
git clone https://github.com/maruki00/SwiftPHP.git
```

2. Install dependencies (if any):

```bash
composer install
```

3. Point your web server to the `/public` folder.

4. Start building your next project with power and speed!

---

## 🛠️ Example

A simple route example:

```php
// routes/web.php

use App\Presentation\Controllers\HomeController;

$router->get('/', [HomeController::class, 'index']);
```

Basic controller example:

```php
// app/Presentation/Controllers/HomeController.php

namespace App\Presentation\Controllers;

class HomeController
{
    public function index()
    {
        return 'Hello, SwiftPHP!';
    }
}
```

---

## 🤝 Contribution Guidelines

We encourage you to contribute to SwiftPHP!

### Especially for Core Contributions:

- The core framework code is located inside `vendor/core/`.
- Follow the DDD architecture standards.
- Maintain clean, simple, and documented code.
- Pull requests should ideally include tests when possible.

**TODO (Help wanted!):**

- [ ] Advanced Routing System
- [ ] Middleware Support
- [ ] Dependency Injection Container
- [ ] CLI Tooling
- [ ] ORM Integration (optional)

Fork, improve, and open a pull request. Let's make SwiftPHP better together! 🚀

---

## 📜 License

SwiftPHP is open-sourced under the [MIT License](LICENSE).

---

**Built for developers who want to move fast — without losing structure. ⚡**
