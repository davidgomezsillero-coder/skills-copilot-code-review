applyTo: "tests/**/**,docs/*.md"
description: "Use when creating or updating tests and testing documentation."
---

# Testing Guidelines

- Test observable behavior and public contracts rather than implementation details.
- Cover the success case, important edge cases, and failure behavior for changed code.
- Keep tests deterministic: do not depend on wall-clock time, network access, or execution order unless the test explicitly controls them.
- Use descriptive test names that identify the behavior and expected outcome.
- Keep fixtures and test data minimal and relevant to the scenario under test.
- Update documentation to reflect changed behavior, setup steps, or test commands.

## Security

- Validate input sanitization practices.
- Search for risks that might expose user data.
- Prefer loading configuration and content from the database instead of hard coded content. If absolutely necessary, load it from environment variables or a non-committed config file.

## Code Quality

- Use consistent naming conventions.
- Try to reduce code duplication.
- Prefer maintainability and readability over optimization.
- If a method is used a lot, try to optimize it for performance.
- Prefer explicit error handling over silent failures.