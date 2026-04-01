# Repository Guidelines

## Project Structure & Module Organization
This repository is currently minimal: no application code, test suite, or Git metadata is present yet. Keep the root focused on project configuration and documentation only.

Recommended layout as the project grows:
- `src/` for application or library code
- `tests/` for automated tests
- `assets/` for static files such as images or sample data
- `docs/` for longer design or usage notes

Prefer small, single-purpose modules. Example: `src/auth/login.py` or `src/components/Button.tsx`.

## Build, Test, and Development Commands
No build or test commands are defined yet. When tooling is added, document the canonical commands here and in the project README.

Expected patterns:
- `npm install` or `pip install -r requirements.txt` to install dependencies
- `npm run dev` or `python -m <package>` to run locally
- `npm test` or `pytest` to execute tests

Avoid ad hoc scripts when a repeatable package-manager command can be added instead.

## Coding Style & Naming Conventions
Use consistent formatting and keep files ASCII unless the project already requires Unicode. Prefer 4 spaces for indentation in Python and 2 spaces only if a JavaScript formatter is configured for that style.

Naming guidelines:
- `PascalCase` for classes and React components
- `camelCase` for variables and functions in JavaScript/TypeScript
- `snake_case` for Python modules, functions, and test files

Adopt a formatter and linter early, such as `prettier` and `eslint`, or `black` and `ruff`.

## Testing Guidelines
Place tests under `tests/` and name them after the unit under test, such as `test_login.py` or `Button.test.tsx`. Add tests with each feature or bug fix. Favor fast, deterministic tests over manual verification.

## Commit & Pull Request Guidelines
Git history is not available in this workspace, so no existing commit convention can be inferred. Use short, imperative commit messages such as `Add login form validation`.

Pull requests should include:
- a clear summary of what changed
- linked issue or task reference when available
- test evidence (`pytest`, `npm test`, screenshots for UI changes)
- notes on setup, migration, or breaking changes
