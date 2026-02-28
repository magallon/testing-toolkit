# Testing Toolkit

A stack-agnostic collection of [Agent Skills](https://agentskills.io) for testing strategy, test generation, and quality assurance in web projects.

## What This Solves

Developers often know *how* to write tests (the syntax of Jest, pytest, JUnit) but struggle with *what* to test, *when*, and *with which type of test*. This toolkit provides AI agents with a structured methodology for making those decisions and, when asked, generating the tests themselves.

It works with **any web stack and testing framework**. The strategy evaluates universal testing principles, not framework-specific syntax.

## Skills

| Skill | Purpose | Status |
|---|---|---|
| **testing-strategy** | Decides what to test, which test type to use, and how to prioritize coverage | ✅ Available |
| *unit-testing* | Generates unit tests following the strategy's recommendations | 🔜 Planned |
| *integration-testing* | Generates integration tests for APIs, data access, and module interactions | 🔜 Planned |
| *e2e-testing* | Generates end-to-end tests for critical user flows | 🔜 Planned |

## Quick Start

### Installation

#### Using the Skills CLI (recommended)

```bash
# List available skills
npx skills add magallon/testing-toolkit --list

# Install the strategy skill
npx skills add magallon/testing-toolkit --skill testing-strategy

# Install all available skills
npx skills add magallon/testing-toolkit --all
```

#### Manual installation

```bash
git clone https://github.com/magallon/testing-toolkit.git

cp -r testing-toolkit/testing-strategy /path/to/your/skills/
```

### Usage

**Get a testing strategy for your project:**
> "Analyze this project and recommend a testing strategy"

**Identify what needs tests:**
> "What are the highest priority things to test in this codebase?"

**Generate tests based on the strategy:**
> "Generate unit tests for the authentication module following the testing strategy"

**Evaluate existing test coverage:**
> "Review my current tests and identify gaps in coverage"

## Stack Compatibility

Works with any web project and testing framework:

- **JavaScript/TypeScript**: Jest, Vitest, Mocha, Testing Library, Playwright, Cypress
- **Python**: pytest, unittest, Robot Framework
- **Java/Kotlin**: JUnit 5, TestNG, AssertJ, Mockito
- **Ruby**: RSpec, Minitest, Capybara
- **PHP**: PHPUnit, Pest, Laravel Dusk
- **Go**: testing package, testify
- **Any other stack** with a testing framework

## Project Structure

```
testing-toolkit/
├── README.md
├── LICENSE
├── CHANGELOG.md
├── CONTRIBUTING.md
│
└── testing-strategy/
    ├── SKILL.md
    └── references/
        ├── test-type-guide.md
        ├── coverage-strategy.md
        └── anti-patterns.md
```

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on reporting issues, proposing new testing checks, and submitting pull requests.

## License

MIT — See [LICENSE](LICENSE) for details.
