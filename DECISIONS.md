# Decisions

This file records durable architectural, workflow, safety, and publishing decisions for Psychometrics Hub. Each entry should include Context, Decision, Rationale, and Consequences.

---

### 2026-05-14 - Consolidate Adult And Pediatric Tools Into psychometrics-hub
Context: Adult and pediatric psychometrics tools lived in separate legacy repos.
Decision: Use `psychometrics-hub` as the destination repo, with `adult/` and `pediatric/` subfolders.
Rationale: One hub simplifies routing and maintenance while preserving the natural audience split.
Consequences: New psychometrics work should default here unless the user explicitly asks for a separate repo.

### 2026-05-14 - Preserve Pediatric Bilingual Files And Redirects
Context: Pediatric tools include `-en` / `-es` variants and redirect files that support older links.
Decision: Preserve those files as-is during consolidation.
Rationale: Reduces risk of broken links and language-routing regressions.
Consequences: Future cleanup should verify redirects and bilingual pages before renaming or deleting files.

### 2026-05-16 - Keep Report Copy Actions Simple
Context: Standard psychometrics report pages had report-copy controls that were cleaned during polish.
Decision: Standard report pages should expose one Detailed Report copy action and one Simple Report copy action; Decisional Capacity and Vanderbilt were intentionally left unchanged.
Rationale: This keeps common pages consistent while respecting tool-specific workflows.
Consequences: Future UI work should check whether a page is a standard report page before applying this pattern.
