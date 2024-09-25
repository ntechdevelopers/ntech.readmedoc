Test-Driven Development (TDD) Cheat Sheet
===================================

**Core Principles**

1. Test First**: 

Always write a failing test before writing the production code.

2. Incremental Development

Take small steps. Write the simplest code to pass the current test, then refactor.

3. Red-Green-Refactor

- Red: Write a test that fails and defines the desired behavior.
- Green: Write the simplest code to pass the test.
- Refactor: Improve code design while keeping tests passing.

**Types of Tests**

1. Unit Tests

- Focus: Smallest testable unit of code (e.g., functions, methods, classes).
- Goal: Verify the correctness of isolated components.

2. Integration Tests

- Focus: Interaction between components or modules.
- Goal: Ensure correct communication and data flow.

3. End-to-End (E2E) Tests

- Focus: Simulate real user interactions with the entire application.
- Goal: Ensure the application works from the user’s perspective.

**Benefits of TDD**

- Enhanced code quality.
- Fewer bugs.
- Increased confidence in code.
- Living documentation.
- Faster feedback loops.

**Test Pyramid**

- Base: Unit tests (fast, numerous, isolated).
- Middle: Integration tests (fewer, slower).
- Top: E2E tests (fewest, slowest).

**Test Doubles**

- Dummy: Placeholder object that fulfills an interface with no implementation.
- Fake: A working object, but not suitable for production (e.g., in-memory database).
- Stub: Provides predefined responses to method calls.
- Mock: A stub with expectations about how it should be called.
- Spy: Wraps around a real object and records interactions for later verification.

**Mockist vs. Classicist TDD**

- London School (Mockist): Heavy use of mocks to isolate units for faster feedback.
- Detroit School (Classicist): Uses real objects and stubs, preferring mocks only when necessary.

**Best Practices**

- Keep Tests Small & Focused: Each test should target a specific behavior (e.g., `testCalculate`, `testSave`).
- Use Descriptive Test Names: Clearly state the purpose (e.g., `testCalculateSumWithPositiveNumbers`).
- Isolate Dependencies: Use test doubles for external systems to create more reliable tests.
- Maintain Test Coverage: Aim for high coverage but focus on critical paths and edge cases.
- Don’t Test Implementation Details: Focus on behavior, not the underlying implementation.
- Refactor Ruthlessly: Clean code is easier to test and maintain.