<!-- Adding or updating an extension? Fill this in. Tooling/CI changes can ignore it. -->

## Extension

- **Name:** newapi-usage
- **Version:** 1.0.0
- **New or update:** new

## What it does

Multi-site NewAPI usage monitor for Muxy. Track balance, total used, and daily usage across multiple NewAPI sites from the status bar, with configurable auto-refresh, balance alerts, and drag-and-drop reordering.

## Permissions

- `commands:exec` — Runs `curl` to fetch data from NewAPI APIs and `cat`/`tee`/`mv` for atomic status cache writes in the background script
- `panels:write` — Updates the status bar with the aggregate balance via `muxy.statusbar.set()`
- `notifications:write` — Shows toast notifications on refresh completion in the popover via `muxy.toast()`
- `storage:read` / `storage:write` — Persists site configurations, balance alert threshold, and cached status data across surfaces (popover ↔ background)

## Checklist

- [x] Directory name equals `manifest.name`.
- [x] `node scripts/validate.mjs newapi-usage` passes locally.
- [x] `README.md` is present with a short description.
- [x] `marketplace.icon` is set (SVG, or square PNG ≥256×256).
- [x] At least one `marketplace.screenshots` entry (PNG, 1600×1000).
- [x] Only permissions actually used are declared.
- [x] Source is readable (not minified/obfuscated).
- [x] Bumped `version` if this updates an existing extension.

## Screenshot / recording

<!-- Drag your listing screenshot(s) here so reviewers can see the extension. -->
