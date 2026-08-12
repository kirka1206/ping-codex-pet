# Ping Codex Pet

Ping is a Codex-compatible v2 animated pet: a calm copper-and-teal otter sentinel with a small amber beacon.

The repository keeps the installable pet package and the QA evidence together so the artifact can be restored or moved without depending on the generation workspace.

## Package

- `pet/pet.json` — Codex pet manifest.
- `pet/spritesheet.webp` — animated sprite atlas.

## QA evidence

- `qa/validation-extended.json` — structural validation (`1536×2288`, 8 columns × 11 rows).
- `qa/chroma-despill-extended.json` — transparency and edge-spill validation.
- `qa/direction-blind-validation.json` — direction-blind validation.
- `qa/direction-semantics.json` — semantic review of all 16 look directions.
- `qa/blind-review-resolution.json` — accepted minor visual-review warnings.
- `qa/look-continuity.json` — look-direction continuity review.
- `qa/standard-review.json` — standard review results.
- `qa/contact-sheet-extended.png` and `qa/look-directions.png` — visual QA sheets.
- `qa/run-summary.json` — generation and validation run summary.

## Restore locally

Copy the contents of `pet/` into the Codex pets directory as `ping` (usually `$CODEX_HOME/pets/ping`, or `~/.codex/pets/ping` when `CODEX_HOME` is unset).
