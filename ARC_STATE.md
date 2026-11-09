# ARC STATE: pgt-website

Live record for this repo. Created automatically 2026-11-09 10:51:09 on first touch (founder SOP:
every repo has a ledger, so when something breaks we can see what decisions were
made instead of guessing). Git HEAD + this file are the truth; chat and memory go stale.

## Step-0 (every session start, enforced by hook)
1. `git status` + `git log --oneline -5` in this repo.
2. Read this file top to bottom (and `canon/SESSION_CONSTITUTION.md` + `docs/ACTIVE_ARCS.md` if present).
3. Check the live state of whatever this repo runs.
4. Emit the STEP 0 block, end with "STOPPED FOR GO", and wait for the founder's go.

## What this repo is
PGT company website: static HTML/CSS, served by GitHub Pages at precisionguessworktech.com (push to main redeploys). Pages: home (site assistant embed), /work.html (portfolio for remote build work), /privacy.html (also FireLine's Play privacy URL), AI App Rescue page. Audience: small businesses, agencies, recruiters.

## Status
| Item | State | Evidence |
|---|---|---|
| work.html footer LinkedIn link | Pushed `68cc457` (main) | Commit on origin/main; live-page check (curl for the profile URL on precisionguessworktech.com/work.html) running at time of writing, result recorded in the next session log line |

| index.html footer LinkedIn link | Pushed `0908d7c` (main) | Commit on origin/main; live check (curl both / and /work.html for the profile URL) running in background at time of writing |

## NEXT
- Confirm the live work page shows the LinkedIn link (if the Pages deploy check failed, re-run it before doing anything else).
- When the PGT LinkedIn company page exists (blocked 11/09: account needs connections), consider linking the company page instead of or alongside the personal profile.

## Decisions (what was decided, why, and the alternative not taken)
- 2026-11-09: LinkedIn link goes in the work.html footer only, next to GitHub, as plain text "LinkedIn", same markup and new-tab behavior. Why: work.html is the page recruiters and agencies land on; footer keeps the layout unchanged (lowest risk). Not taken: a button in the hero/contact section (more visible, but a layout change the founder didn't ask for) and adding it to every page (scope creep).

## AI log (where the AI was wrong or risky, and how it was caught)

## Session log
- 2026-11-09: commits this session: `68cc457` (work.html footer link), `8452891` (ledger), `0908d7c` (index.html footer link + ledger). Evidence so far: all pushed to origin/main; live-page confirmation pending (NEXT item 1). Next: confirm both live pages, then nothing further on this repo until the LinkedIn company page exists.
- 2026-11-09: founder asked to add the LinkedIn link to the home page too. Added to index.html footer between GitHub and the Facebook icon, plain text like GitHub. Decision: text link, not an icon like Facebook (no new SVG to maintain; matches GitHub next to it). Not taken: a LinkedIn icon matching the Facebook one.
- 2026-11-09: founder GO. Added a LinkedIn link (linkedin.com/in/les-fleming-55736344a) to the work.html footer next to GitHub. Founder approved LinkedIn presence 11/09 (reversed the earlier no-LinkedIn rule).
- 2026-11-09 10:51:09: ledger created on first touch. Mechanical record of every change: `docs/ACTIVITY_LOG.md`.
