# Project Rules

## Coding
- Keep changes focused and follow the existing plain HTML, CSS, and JavaScript approach unless the project is intentionally changing frameworks.
- Preserve the established page design and responsive behavior.
- Use semantic HTML, accessible labels, and keyboard-operable controls.
- Reuse existing patterns and utilities; avoid adding dependencies without a clear need.
- When changing persisted task data, keep older saved data compatible and preserve unrelated task fields.
- Treat task text and notes as untrusted input. Render them with `textContent` and DOM APIs; do not interpolate them into `innerHTML`.

## Naming
- Use lowercase kebab-case for filenames, directories, CSS classes, and HTML IDs.
- Use camelCase for JavaScript variables and functions.
- Use UPPER_SNAKE_CASE for constants.
- Choose descriptive names that reflect the behavior or data they represent.

## Testing and Validation
- Write a test for every endpoint you create, and always validate that these endpoints are working.
- Cover endpoint success cases, relevant invalid inputs, and expected error responses.
- For browser features, test the user interaction, persistence across reloads when applicable, and responsive layout.
- After every change, test adding, editing, and deleting tasks and writing notes in the browser; refresh the page and verify the changes and notes are still saved.
- Add or extend focused tests for behavior changes. If no automated test setup exists, perform and report a focused manual browser check.
- Run relevant tests and checks after changes; report any checks that could not be run.
