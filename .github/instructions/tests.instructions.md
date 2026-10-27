---
applyTo: "tests/**"
---

# Test instructions

- Write a failing test before implementing a behavior change.
- Never weaken or delete an existing assertion.
- Unit tests should call services directly with mocked repositories; avoid HTTP and database dependencies.
- Integration tests should exercise the API with `TestClient` and a real PostgreSQL database.
- Use the repository's pytest configuration; `asyncio_mode = "auto"` means async tests do not need `@pytest.mark.asyncio`.
