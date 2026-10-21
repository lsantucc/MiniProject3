# Validation Reflection — lsantucc

**Validator:** lsantucc | **Project owner:** pstorch1 | **Projects reviewed:** 10

## Note on scope

My partner's MiniProject2 repository contains only the Part 1 commit data, so there were no author labels to compare against. Every record was a pre-discussion disagreement (0% agreement). My values were used as the final values (100% post-discussion agreement, all ValidatorKept). The labels discussed below were built from pstorch1's WoC commit data (mapped back to each project's GitHub history) and from the current GitHub commit logs.

## What precedes long gaps

Across the ten projects, the long gaps were rarely preceded by visible trouble such as unanswered bug reports. They usually followed the end of a work cycle by a small core team. In gnuradio_gr-inspector, the last commits before its 24-month gap (2020-03 to 2022-02) are one developer finishing a port to GNU Radio 3.8: "Update documentation to GR 3.8 version," then MANIFEST fixes. In adibender_pammtools, the gap starts right after a release cycle (site build for 0.5.8, "Update news + description"). In openworm_sibernetic, the gap follows a burst of CI configuration work by a single maintainer. The common signal is concentration: a project where one person makes nearly all recent commits, and those commits are wrap-up work (docs, release, build config) rather than new features. unity-technologies_synthdet shows the terminal version of this. Its last meaningful work was an engine upgrade in 2022, followed only by broken-link fixes.

## What triggers recovery

Recovery came from two sources. The first was **new contributors adapting the project to a changed ecosystem**. gr-inspector was revived by Bjoern Kerler and Ryan Volz porting it to GNU Radio 3.10 and adding a conda recipe. sibernetic resumed when a new contributor (Austin Klein) began README and CI work on a new version branch. The second was the **original maintainer returning for a release**. pammtools came back when Andreas Bender fixed reported issues (#226, #230) and prepared a CRAN release. brainrender's rebound coincided with its move to the brainglobe organization, which brought documentation work, dependency modernization, and automated pre-commit bot activity. In every recovered case, the first post-gap commits were maintenance or porting, not new features. Projects come back by first becoming buildable and current again.

## When gaps don't mean project death

Several "gaps" were not dormancy at all. cp2k_cp2k's longest gap is one month in 2001, and it has produced roughly 2,000 commits per year for 25 years. schnetpack's single empty month is December 2024, a holiday lull, and normal bug-fix work resumed in January. rub-nds_tls-attacker and gigascience_gigadb-website have no empty months at all. Even a long gap did not mean death for gr-inspector: it was quiet for two years, then revived. It is now marked Inactive only because its last commit (2025-03-03) falls just before the codebook cutoff. In contrast, SynthDet's single commit after a 16-month gap did not signal life. The content of post-gap commits mattered more than their count.

## Interpretation pitfalls and how I resolved them

1. **Trivial gaps and HasRecovered.** The codebook asks whether the project became active after the *longest* gap, but very active projects still have a "longest" gap of one or two months. A literal reading labels cp2k, schnetpack, and drizzlepac as "recovered." I recorded "Yes" with evidence noting the gap length, and would propose a 3-month minimum (matching the MiniProject2 gap definition) to resolve this consistently.
2. **One commit is not recovery.** SynthDet technically resumed after its gap, but the only commit removed a dead link. I labeled HasRecovered "No" and ActivityPattern "stopped."
3. **Pattern labels depend on the time window.** brainrender looks U-shaped through 2024 but falls again afterward. drizzlepac looks "rising" around 2019 and "declining" since. I chose "irregular" when a single trend did not hold across the full timeline.
4. **Data source mismatch.** WoC data and live GitHub history differ: WoC includes commits from forks and rewritten history (cp2k's WoC count is about 2x its GitHub count), and GitHub has commits after the WoC snapshot. I used WoC for gap and pattern analysis and GitHub for CurrentStatus and RecentThemes, as the instructions specify.
5. **Theme ambiguity.** Merge commits, CI workflow edits, and Python-version bumps do not fit cleanly into the theme list. I classed version and pin changes as Dependency updates and CI configuration as Other.

## Suggested codebook improvements

- Set a minimum gap length (for example, 3 months) before HasRecovered and WhyRecovered apply, and add an explicit "N/A – no significant gap" value.
- Make the CurrentStatus values consistent: the codebook lists "yes/no" but defines "Active/Inactive."
- Specify a snapshot date for RecentThemes, since a project's last 10 commits change over time.
- Say how to count merge commits and CI/workflow changes when picking themes.
