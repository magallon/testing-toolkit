# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).


## [1.1.0] - 2026-03-14

### Added
- `e2e-testing` skill with browser automation patterns
  - Page Object Model patterns in pseudocode (stack-agnostic)
  - Framework selection guide (Playwright, Cypress, Selenium, Laravel Dusk, Capybara)
  - Selector strategy, wait patterns, auth state reuse, test data management
  - Network mocking, visual regression, accessibility testing patterns
  - Flaky test diagnosis flowchart with fix-one-at-a-time protocol
  - CI/CD pipeline templates for GitHub Actions, GitLab CI, and generic systems
  - Three output modes: Design, Generation, Fix

### Changed
- `testing-strategy` now covers unit, integration, and component test generation (no separate skills needed)
- Updated README with new skill table and project structure


## [1.0.0] - 2025-02-27

### Added
- Initial release of the Testing Toolkit
- `testing-strategy` skill with testing pyramid methodology
  - Test type decision framework (unit, integration, component, E2E)
  - Coverage prioritization strategy (critical paths → business logic → edge cases)
  - Mocking strategy guidelines
  - Hybrid mode: recommends strategy and generates tests on request
- Reference materials for test type guide, coverage strategy, and anti-patterns
- Full documentation (README, CONTRIBUTING, LICENSE)
