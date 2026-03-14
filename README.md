# Testing Toolkit

A stack-agnostic collection of [Agent Skills](https://agentskills.io) for testing strategy, test generation, and quality assurance in web projects.

## What This Solves

Developers often know *how* to write tests (the syntax of Jest, pytest, JUnit) but struggle with *what* to test, *when*, and *with which type of test*. This toolkit provides AI agents with a structured methodology for making those decisions and, when asked, generating the tests themselves.

It works with **any web stack and testing framework**. The strategy evaluates universal testing principles, not framework-specific syntax.

## Skills

| Skill | Purpose | Status |
|---|---|---|
| **testing-strategy** | Decides what to test, which test type to use, and how to prioritize coverage. Generates unit, integration, and component tests on request. | ✅ Available |
| **e2e-testing** | Generates end-to-end tests for critical user flows with Page Object Model, wait patterns, flaky test diagnosis, and CI/CD integration. Stack-agnostic. | ✅ Available |

## Quick Start

### Installation

#### Using the Skills CLI (recommended)

```bash
# Interactive install — choose which skills and agent
npx skills add magallon/testing-toolkit

# List available skills before installing
npx skills add magallon/testing-toolkit --list
```

#### Install to a specific agent

```bash
# Install to a specific agent
npx skills add magallon/testing-toolkit --skill testing-strategy -a claude-code
```

#### Install all skills to all agents

```bash
# Install everything to every detected agent (no prompts)
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
├── testing-strategy/
│   ├── SKILL.md
│   └── references/
│       ├── test-type-guide.md
│       ├── coverage-strategy.md
│       └── anti-patterns.md
│
└── e2e-testing/
    ├── SKILL.md
    └── references/
        ├── framework-guide.md
        ├── page-object-patterns.md
        ├── patterns-and-anti-patterns.md
        └── ci-pipeline-templates.md
```

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on reporting issues, proposing new testing checks, and submitting pull requests.

## License

MIT — See [LICENSE](LICENSE) for details.
