# Decisions

Why things are the way they are. Read this before reopening a decision.
Newest first. One entry per decision; do not rewrite old entries, add a new
one that replaces them.

## Entry format

```
## YYYY-MM-DD: short title
Decision: what was decided, in one sentence.
Why: the reason, and what it costs.
Rejected: the alternatives considered and why they lost.
```

## Entries

## 2024-11-11: Use Vue 3 with Vite and TypeScript
Decision: Use Vue 3 framework with Vite as the build tool and TypeScript for type safety.
Why: Vue 3 offers a modern, component-based architecture. Vite provides fast development server and build. TypeScript adds type checking for better maintainability.
Rejected: React (user preference for Vue), Plain JS (less maintainable at scale), Svelte (less ecosystem support for this use case).

## 2024-11-11: Use Tailwind CSS for styling
Decision: Use Tailwind CSS utility-first framework for all frontend styling.
Why: Rapid development, consistent design, and no need to write custom CSS. Reduces file size and maintenance overhead.
Rejected: Plain CSS (too verbose for large projects), Bootstrap (too opinionated, harder to customize), Sass (requires compilation step).

## 2024-11-11: Static frontend first
Decision: Start with static HTML/CSS/JS frontend before building the backend.
Why: Allows quick iteration on UI/UX. Login page can be developed and tested visually before connecting to authentication logic.
Rejected: Building backend first (delays visual feedback), full-stack from day one (too complex for initial setup).
