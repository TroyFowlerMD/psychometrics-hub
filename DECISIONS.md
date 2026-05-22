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

### 2026-05-22 - Explain Repo Work With Beginner Context
Context: Dr. Fowler is new to Git, GitHub, GitHub Desktop, Codex, and local-vs-remote repository workflows.
Decision: Codex should explain repo work with extra beginner-friendly context by default, including definitions, why each step matters, exact local paths/button names when useful, and a clear distinction between local files, local commits, pushed GitHub commits, pull requests, and deployed site changes.
Rationale: Better context reduces accidental duplicate clones, OneDrive/Git confusion, and uncertainty about whether work is local, synced, or live.
Consequences: Future repo instructions and shutdown summaries should favor plain outcome language and step-by-step guidance over unexplained Git shorthand.

### 2026-05-22 - Surface Workflow Streamlining Opportunities
Context: Dr. Fowler wants Codex to notice chances to make his coding, GitHub, GitHub Desktop, deployment, and cross-machine workflows smoother.
Decision: When Codex sees a practical workflow improvement, it should present the opportunity proactively with the expected benefit, any risk or cost, and the smallest safe next step.
Rationale: Small workflow improvements compound, especially while Dr. Fowler is learning Git and using Codex across multiple machines.
Consequences: Future sessions should separate optional workflow suggestions from required task work so recommendations help without derailing the current task.
