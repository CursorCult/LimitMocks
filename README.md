# LimitMocks

Prefer real dependencies; use mocks sparingly.

**Install**

```sh
pipx install cursorcult
cursorcult link LimitMocks
```

Rule file format reference: https://cursor.com/docs/context/rules#rulemd-file-format

**When to use**

- You want tests to resemble reality, but occasional mocks are unavoidable.
- You’re worried about over‑mocked suites giving false confidence.
- You want a middle ground between full integration tests and pure unit tests.

**What it enforces**

- Real implementations are the default in tests.
- Mocks are limited to truly impractical dependencies.
- Core logic is never mocked away.

See also: https://github.com/CursorCult/NoMocksNoSkips.git

**Credits**

- Developed by Will Wieselquist. Anyone can use it.
