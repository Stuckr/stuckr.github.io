# PBLax Scorekeeper — Project Rules

## OVERVIEW

This is a single-file, self-contained lacrosse scorekeeper. `index.html` is the entire app: all CSS and JavaScript are inline. It runs directly from `file://` with no server, build step, or companion assets.

## WORKING FILE & BACKUPS

- Working file (edit this from now on): `Z:\PBInput\PBLax scorekeeper\index.html`
- Backup directory: `Z:\PBInput\PBLax scorekeeper\backup`
- Always save a pre-edit snapshot to the backup directory, never to the temp folder.
- Name backups descriptively, e.g. `index.pre-<change-name>.html`.

## SINGLE-FILE CONSTRAINT

- The app must remain one self-contained file.
- Do not add external dependencies: no `<link>`, `<script src>`, `@import`, `url()`, `<img>`, `fetch`, or other companion assets.
- Verify the file still opens and works from `file://` after any change.

## WORKFLOW

- Keep responses concise and to the point.
- For changes: use subagents to implement where possible; act as coordinator.
- Use brainstorming before new features or behavior changes, and systematic-debugging before fixes.
- Test every change in a browser (headless Chrome via CDP works well), confirm zero console errors, and run the relevant regression suites plus a syntax check.
- Do not assume changes work — verify and report evidence.

## STABLE BEHAVIOR

Unless explicitly asked to change: preserve the fixed core event-button grid, format-specific buttons, roster-based goalie selection and save attribution, per-goalie summary rows, full-history auto-scrolling ticker, penalty flows, and light/dark themes.
