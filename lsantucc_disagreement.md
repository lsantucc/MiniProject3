# Disagreement — lsantucc / pstorch1

**Validator:** lsantucc | **Project owner:** pstorch1

## How disagreements were resolved

pstorch1's MiniProject2 repository (Durza14/MiniProject2) contains only Part 1 output. It has no values for HasRecovered, WhyRecovered, ActivityPattern, CurrentStatus, or RecentThemes. Every one of the 50 records therefore counts as a pre-discussion disagreement (AuthorValue "Not reported" vs. a validator value). No discussion with the owner was possible, so my values were used as the final values. All 50 records are resolved as **ValidatorKept** (see `lsantucc_disagreement_resolution.csv`).

The examples below are the records where a second coder could most reasonably have disagreed with me, and how I settled each one from the evidence.

## Example 1 — cp2k/cp2k (HasRecovered)
**Author:** Not reported
**Validator:** Yes
**Parties:** lsantucc (validator), pstorch1 (owner, no values)
**Reason:** The longest zero-commit stretch is one month (2001-09), in the project's first months. A literal codebook reading gives "Yes" because activity resumed. A second coder could argue "No," since the project never really went dormant. It has 50,131 commits after the gap, from the same authors (Chris Mundy, Juerg Hutter).
**Resolution:** ValidatorKept ("Yes"), with the gap length recorded in KeyEvidence. The same reasoning applies to schnetpack (1-month gap) and drizzlepac (2-month gap).

## Example 2 — Unity-Technologies/SynthDet (HasRecovered)
**Author:** Not reported
**Validator:** No
**Parties:** lsantucc (validator), pstorch1 (owner, no values)
**Reason:** One commit followed the 16-month gap (2023-08 to 2024-11), so a literal reading could call it recovered. That commit (2024-12-05) only "removed dead dataset link." Nothing has come since, and yearly commits fell 267 → 138 → 4 → 2 → 1.
**Resolution:** ValidatorKept ("No"). A single maintenance commit is not recovery, and ActivityPattern is "stopped."

## Example 3 — brainglobe/brainrender (ActivityPattern)
**Author:** Not reported
**Validator:** irregular
**Parties:** lsantucc (validator), pstorch1 (owner, no values)
**Reason:** Yearly commits (272 / 613 / 81 / 49 / 166 / 242 / 44 / 46) dip in 2021-22 and rebound in 2023-24, which looks U-shaped. Activity then falls again in 2025-26.
**Resolution:** ValidatorKept ("irregular"). Judged over the full timeline, no single trend holds. "U-shaped" would only fit if the series stopped at 2024.
