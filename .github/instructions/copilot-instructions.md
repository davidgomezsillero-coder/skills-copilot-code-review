# Repository Instructions

- Keep changes focused on the requested behavior and preserve existing project conventions.
- Do not revert or overwrite user changes that are unrelated to the task.
- Prefer small, readable implementations over unnecessary abstractions or premature optimization.
- Reuse existing patterns and dependencies before introducing new ones.
- Validate changed behavior with the most focused available test, lint, or type-check command.
- Update relevant tests and documentation when behavior, configuration, or setup changes.
- Follow the scoped instructions in `.github/instructions/` for backend Python code, tests, and documentation.

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
