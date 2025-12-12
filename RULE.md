---
description: "Prefer real dependencies; use mocks sparingly"
alwaysApply: true
---

# LimitMocks Rule

Minimize use of mocks in tests; prefer real implementations.

Requirements:
1. Default to testing against real code paths and real implementations of dependencies.
2. Introduce a mock or stub only when the real dependency is impractical to use in tests (for example: nondeterministic, prohibitively slow, unavailable), and limit the mock to the smallest surface necessary.
3. Do not mock core logic of the unit under test; mocks may only stand in for external dependencies.
4. If mocks are used for a dependency, ensure at least one test path exercises the real dependency or real integration behavior.
