# Ping Codex Pets

Ping is a Codex-compatible v2 animated pet: a calm copper-and-teal otter sentinel with a small amber beacon.
Hex is a Codex-compatible v2 animated pet: an evil swamp-witch honey badger with a mossy mantle, amber talisman, and poisonous green magic.

The repository keeps the installable pet package and the QA evidence together so the artifact can be restored or moved without depending on the generation workspace.

## Packages

- `pet/pet.json` and `pet/spritesheet.webp` — the original Ping package.
- `pet/hex/pet.json` and `pet/hex/spritesheet.webp` — the Hex package.
- `pet/hex/spritesheet.png` — the exact transparent PNG source used for upload and validation.

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
- `qa/hex/` — Hex validation reports, direction sheets, and motion previews.

## Restore locally

Copy the contents of `pet/` into the Codex pets directory as `ping` (usually `$CODEX_HOME/pets/ping`, or `~/.codex/pets/ping` when `CODEX_HOME` is unset). Copy `pet/hex/` as the separate `hex` pet directory.
