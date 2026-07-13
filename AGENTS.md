# Repository Guidelines

## Project Structure & Module Organization

This is a GitHub profile repository rather than an application. The root `README.md` is the published profile and currently contains all user-facing content. It combines Markdown headings and lists with HTML for centered layouts, badge groups, and externally hosted statistics. Keep repository-level contributor instructions in `AGENTS.md`. If local images are introduced, place them in a clearly named directory such as `assets/` and reference them with relative paths.

## Build, Test, and Development Commands

There is no package manager, build pipeline, or automated test suite. Review changes with standard Git tools:

- `git diff --check` detects trailing whitespace and malformed conflict markers.
- `git diff -- README.md` shows the exact profile changes under review.
- `git status --short` confirms that only intended files are included.

Before submitting, preview `README.md` in a GitHub-compatible Markdown renderer. Verify that headings, separators, centered blocks, badges, and statistics images display correctly.

## Coding Style & Naming Conventions

Use clear Markdown headings in descending order and keep related profile content grouped into short sections. Match the existing HTML style: two-space indentation inside nested blocks, lowercase element names, double-quoted attributes, and self-closing `<img />` tags. Every image must have concise, meaningful `alt` text. Prefer HTTPS image URLs and avoid adding scripts or opaque tracking links. Use lowercase, hyphenated names for new assets, for example `assets/profile-banner.png`.

## Testing Guidelines

Treat visual rendering as the primary test. Check the README at desktop and narrow widths, confirm every external image loads, and ensure links reach their intended destinations. Run `git diff --check` for every change. When editing repeated badge markup, inspect each `alt`, `src`, and closing tag individually.

## Commit & Pull Request Guidelines

Recent history uses short, imperative subjects such as `Update README.md` and `Delete GitHub Trophies section`. Follow that pattern: keep each commit focused and describe the visible outcome. Pull requests should explain the profile change, identify any new external services or assets, and include a rendered screenshot when layout changes are significant. Link a relevant issue when one exists, and avoid mixing unrelated profile edits in the same PR.
