<!-- last-reviewed: 2026-05-19 -->
<!-- source: repository-and-memory -->

# Psychometrics Hub

## Snapshot
Consolidated repo for adult and pediatric psychometrics tools. The hub is a static GitHub Pages site with separate `adult/` and `pediatric/` folders.

## Current Structure
- `index.html`: root hub for the merged repo
- `adult/`: adult dashboard and tool pages
- `pediatric/`: pediatric dashboard, bilingual tool pages, and redirect files

## Source Mapping
- `adult-psychometrics` -> `adult/`
- `pediatric-psychometrics` -> `pediatric/`

## Merge Notes
- Legacy source repos were not modified during consolidation.
- Adult and pediatric collections stay in separate folders to keep navigation clear and reduce breakage risk.
- Pediatric `-en` / `-es` files were preserved as-is.
- Pediatric redirect files like `gad7.html` were preserved so old intra-folder links still resolve.

## Maintenance Notes
- Keep public pages free of source-repo/migration wording.
- Verify rendered page structure when changing user-facing pages; HTTP 200 is not enough.
- Standard psychometrics report pages should keep the simplified copy-action pattern unless a tool has its own intentional workflow.
