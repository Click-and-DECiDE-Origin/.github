# Click and DECIDE Organization Guidelines

## Architecture & Code Standards

- **Strong & Strict Typing**: When working in statically typed languages, enforce strict mode, disallow untyped escape hatches (e.g., `any` or raw dynamic objects), and define explicit contracts/DTOs for all input/output payloads.
- **Language Idioms**: Adhere strictly to idiomatic patterns, official style guides, and ecosystem best practices for the specific language of each repository.
- **Modularity & Decoupling**: Separate business logic, transport layers, and data access. Rely on dependency injection and pure functions where applicable.
- **Security & Data Sanitization**: Prevent SQL injection and command injection. Always sanitize inputs, use parameterized queries, and never hardcode secrets, credentials, or internal connection strings.
- **Testing**: Include unit test coverage for pure utility functions, parsing routines, and domain transformations.

## Behavioral Rules for Copilot

- **Concise Outputs**: Provide direct, minimal, production-ready code diffs without conversational filler.
- **Minimal Dependencies**: Do not introduce third-party libraries if functionality is readily achievable using the project's existing dependencies or native language APIs.
- **Respect Context**: Before refactoring or proposing new code, inspect existing patterns and folder structures in the repository to maintain consistency.
- **Safety First**: Prohibit generating destructive shell scripts or operations that bypass code reviews or testing pipelines.
