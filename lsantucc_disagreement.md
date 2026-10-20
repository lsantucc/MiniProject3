# Disagreement Examples — lsantucc (validator) / pstorch1 (project owner)

## Status

No owner-vs-validator disagreements could be recorded. pstorch1's MiniProject2 repository (Durza14/MiniProject2) contains only Part 1 output (WoC commit retrieval and GitHub stats). There is no project stats file, time series, or reflection, and no values for HasRecovered, WhyRecovered, ActivityPattern, CurrentStatus, or RecentThemes. With no AuthorValue to compare against, no disagreements exist and no discussion could be held. The instructor was notified on 2026-10-19.

## Cases I would have raised in discussion

These are the labels in my validation log where I expect a second coder could reasonably disagree. These are the cases I would bring to an evidence-based discussion.

### 1. cp2k_cp2k — HasRecovered (my value: Yes)
- **Issue:** The longest zero-commit stretch is a single month (2001-09), in the project's first months. Activity resumed right after, so a literal reading of the codebook gives "Yes." An equally defensible reading is "No / N/A," because the project never went dormant.
- **Evidence:** 50,131 commits after the gap. The same authors (Chris Mundy, Juerg Hutter) committed before and after. There is no README or issue sign of an interruption.
- **How I'd resolve it:** Agree on a minimum gap length (for example, 3+ months, matching the MiniProject2 gap definition) before HasRecovered applies. Under that rule the value becomes "No significant gap." The same reasoning applies to atomistic-machine-learning_schnetpack (1-month gap, 2024-12) and spacetelescope_drizzlepac (2-month gap, 2009).

### 2. unity-technologies_synthdet — HasRecovered (my value: No)
- **Issue:** One commit followed the 16-month gap, so a literal reading could say it recovered.
- **Evidence:** The only post-gap commit (2024-12-05) is "removed dead dataset link." There has been nothing since, and yearly commits fell 267 → 138 → 4 → 2 → 1.
- **How I'd resolve it:** A single maintenance commit is not recovery. I would keep "No" and label ActivityPattern "stopped."

### 3. brainglobe_brainrender — ActivityPattern (my value: irregular)
- **Issue:** The yearly series (272 / 613 / 81 / 49 / 166 / 242 / 44 / 46) has a clear dip in 2021-22 and a rebound in 2023-24, which looks U-shaped. Activity then falls again in 2025-26.
- **Evidence:** The rebound lines up with the project moving to the brainglobe organization (README and developer-guide updates by Adam Tyson in June 2023).
- **How I'd resolve it:** Compare the plot over the full timeline rather than one window. Because there is a second decline, I chose "irregular." "U-shaped" would be a reasonable compromise if the class judged the trend only up to 2024.
