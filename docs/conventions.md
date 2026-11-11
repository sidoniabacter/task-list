# Conventions

How code is written and committed here. Read this before writing code or
making a commit.

## Language

- Code and comments: English
- Commit messages: English, imperative mood
- Documentation (docs/): Romanian for project docs, English for technical specs

## Code style

- Vue 3 Single File Components (.vue) with `<script setup>` syntax
- TypeScript for all JavaScript code
- Tailwind CSS utility classes for styling
- 2-space indentation
- Semicolons in JavaScript/TypeScript
- Single quotes for strings
- Comma-dangle: true (trailing commas)
- Prefer composition API over options API

## Branches

- main: always deployable, protected.
- feature/*: one branch per feature, named feature/short-description (e.g., feature/login-page).
- bugfix/*: one branch per bug fix, named bugfix/short-description.

## Commit messages

One line in the imperative, under 72 characters: "Add login form with Tailwind styling".
For larger changes, use a body to explain the what and why.

## File naming

- Components: PascalCase (LoginForm.vue)
- Utilities/functions: camelCase (apiClient.ts)
- CSS classes: kebab-case (tailwind handles this)
