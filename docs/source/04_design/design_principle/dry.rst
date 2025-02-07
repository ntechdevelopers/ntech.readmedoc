DRY
===================================

The DRY (Don't Repeat Yourself) principle means that every piece of knowledge should only exist once in your codebase. Sounds great, right?

But when does DRY become TOO DRY?
Sometimes, in an effort to eliminate all repetition, we can end up over-abstracting our code. This can lead to code that is hard to understand, maintain, or extend. For example, if you find yourself creating overly generic methods or classes that try to handle too many scenarios, you might be taking DRY too far. This makes the code confusing for others (or even your future self) and increases the chance of introducing bugs when changes are needed.

DRY isn't always the best choice. In cases like DTOs or database schemas, repetition can be more readable and clear. Reusing too much can make your design rigid and harder to change when requirements evolve.

**Pros of DRY:**

- Reduces repetition, making your code easier to maintain.
- Less copy-pasting means fewer chances for mistakes and errors.
- Changes in logic require fewer edits, which reduces the risk of bugs.

**Cons of DRY:**

- Too much abstraction can make your code hard to understand.
- Reusing too much logic across different parts can make changes risky and cause unexpected problems.