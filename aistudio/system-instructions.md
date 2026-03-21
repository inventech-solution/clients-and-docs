## UI & Design Rules

- Use SVG icons exclusively. No emojis anywhere in the interface.
- Spacing, padding, and margins should be refined and compact — avoid excessive whitespace, oversized gaps, or large border radii. Aim for a dense, professional layout.
- All navigation labels, button text, and UI copy must use plain, everyday language. Write for non-technical end users, not developers.

## Floating Action Button (FAB)

- Include a floating action button on screen during development for API/setup actions (e.g. creating a new collection or document).
- FAB should point to endpoints at apis.inventechsolution.com.
- On click, play a brief click/pulse animation on the button.
- When there are no actions to execute, set the FAB to display: none.

## File Size & Code Organisation

- No single file should exceed 200 lines of code.
- If a file grows beyond 200 lines, split it into smaller, focused files — by feature, component, or responsibility.
- Each file should do one thing well. Avoid monolithic files that mix unrelated logic or UI.

## features.md (Mandatory)

- Always create and maintain a features.md file in the project root.
- This file is the single source of truth for the entire application. Any human or AI reading it should fully understand the app — what it does, how to use it, where to go, and what each feature does.
- features.md must include:
  - Every feature and sub-feature with a clear explanation
  - Use cases for each feature
  - Status of each feature: Complete / In Progress / Pending
  - Any half-built or incomplete features, clearly flagged
  - Planned production-ready features not yet built
- Keep features.md updated after every change to the app.
