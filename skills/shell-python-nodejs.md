# Shell, Python, Node.js Skill

## Overview
Expertise in scripting and development with Shell, Python, and Node.js.

## Shell Scripting (Bash)

### Best Practices
- Use `set -euo pipefail` at the top
- Quote variables: `"$var"`
- Use `[[ ]]` for conditionals
- Prefer `$()` over backticks
- Use functions for reusability

### Common Patterns
- Argument parsing with `getopts`
- Error handling with `trap`
- File operations with `find`, `xargs`
- Process management with `ps`, `pgrep`

### Advanced Features
- Arrays: `arr=(a b c)`
- Parameter expansion: `${var:-default}`
- Process substitution: `<(command)`
- here-documents for multi-line text

## Python

### Best Practices
- Follow PEP 8 style guide
- Use type hints
- Virtual environments (`venv`)
- Docstrings for functions/classes
- Exception handling with specific exceptions

### Common Patterns
- List/dict comprehensions
- Context managers (`with` statements)
- Generator functions
- Decorators for cross-cutting concerns

### Data Processing
- Pandas for data manipulation
- NumPy for numerical operations
- JSON handling with `json` module
- CSV processing with `csv` module

### Testing
- `unittest` or `pytest`
- Mock with `unittest.mock`
- Fixture patterns
- Parameterized tests

### Async Programming
- `async`/`await` syntax
- `asyncio` event loop
- Concurrent futures
- Async HTTP clients (aiohttp, httpx)

## Node.js

### Best Practices
- Use `const`/`let` instead of `var`
- Async/await for async operations
- Error handling with try/catch
- Modular code with ES modules
- Environment variables with `dotenv`

### Common Patterns
- Event-driven programming
- Stream processing
- Callback patterns (legacy)
- Promise chains

### Web Development
- Express.js for REST APIs
- Middleware patterns
- Error handling middleware
- CORS configuration

### Testing
- Jest for unit/integration tests
- Supertest for API testing
- Mocking with `jest.mock`
- Test doubles (spies, stubs, mocks)

### Performance
- Event loop understanding
- Non-blocking I/O
- Cluster module for multi-core
- Memory management

## Cross-Language Patterns

### File Operations
- Shell: `cat`, `grep`, `awk`
- Python: `open()`, `pathlib`
- Node.js: `fs` module

### HTTP Requests
- Shell: `curl`, `wget`
- Python: `requests`, `httpx`
- Node.js: `axios`, `node-fetch`

### JSON Processing
- Shell: `jq`
- Python: `json` module
- Node.js: `JSON.parse/stringify`

### Configuration
- Environment variables
- Config files (YAML, JSON, TOML)
- Command-line arguments

## CI/CD Integration

### Shell
- Build scripts
- Deployment automation
- Health checks

### Python
- Test runners
- Data processing pipelines
- Automation scripts

### Node.js
- Build tools (Webpack, Vite)
- Package management
- Test execution

## Security Best Practices

- Input validation
- Sanitize user input
- Avoid shell injection
- Use secure libraries
- Update dependencies regularly
- Environment variable security
