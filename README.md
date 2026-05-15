# psychometrics-hub

Local destination repo for the merged psychometrics tools portfolio.

## Current structure

- `index.html`: root hub for the merged repo
- `adult/`: adult dashboard and tool pages
- `pediatric/`: pediatric dashboard, bilingual tool pages, and redirect files

## Source mapping

- `adult-psychometrics` -> `adult/`
- `pediatric-psychometrics` -> `pediatric/`

## Merge notes

- The legacy source repos were not modified.
- The adult and pediatric collections stay in separate folders to keep navigation clear and reduce breakage risk.
- Pediatric `-en` / `-es` files were preserved as-is.
- Pediatric redirect files like `gad7.html` were preserved so old intra-folder links still resolve.
