# psychometrics-hub

Consolidated psychometrics hub for adult and pediatric screening/assessment tools. The repo keeps adult and pediatric collections in separate folders while publishing as one GitHub Pages project.

## Current Structure

- `index.html`: root hub for the merged repo
- `adult/`: adult dashboard and tool pages
- `pediatric/`: pediatric dashboard, bilingual tool pages, and redirect files

## Source Mapping

- `adult-psychometrics` -> `adult/`
- `pediatric-psychometrics` -> `pediatric/`

## Merge Notes

- The legacy source repos were not modified.
- The adult and pediatric collections stay in separate folders to keep navigation clear and reduce breakage risk.
- Pediatric `-en` / `-es` files were preserved as-is.
- Pediatric redirect files like `gad7.html` were preserved so old intra-folder links still resolve.

## Project Files

- `CONTEXT.md`: Short session-start briefing for Codex and returning developers.
- `TASKS.md`: Live working task list seeded from repository state and migrated project memory.
- `WORKLOG.md`: Append-only session-end worklog format.
- `DECISIONS.md`: Key consolidation and workflow decisions.
- `docs/psychometrics-hub.md`: Hub-level project context and maintenance notes.
