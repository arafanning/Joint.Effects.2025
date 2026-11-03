# Published Joint Effects (2025): syntax recovery status

**Status: Original final analysis syntax not yet recovered.** This note documents the repository audit and a conservative recovery plan. It is not an independently executable analysis or a claim of replication.

## Current inventory

The existing `01_setup.R` to `06_tables_figures.R` files have not been modified. `01_setup.R` only establishes local output folders and a random seed. The remaining five are brief templates with no implemented analysis models. The repository's README explicitly identifies the files as **an incomplete scaffold**.

The authoritative paper is Adams et al. (2025), *Joint effects of human immunodeficiency virus (HIV) and cannabis on neurocognition*, *Neuropsychology, 39*(6), 473–489. DOI: https://doi.org/10.1037/neu0001003. The full study data are restricted.

## Research questions that any recovered source code needs to reproduce

- HIV-positive and HIV-negative participants crossed with cannabis-use status, comparing four groups in the approximately 269-person analytic sample.
- Group comparisons for global and domain-specific neurocognitive **mean performance**, separately from impairment classifications.
- Domain-specific impairment models, which must not be inferred from the nonsignificant omnibus mean differences.
- The cannabis-user-only analysis of amounts of recent cannabis use in relation to neurocognition, with particular attention to HIV-status differences.
- Preprocessing, standardization, exclusions and sample Ns, direction of cognitive indicators, covariates, and diagnostics as documented in the final paper.
- Tables, effect sizes, uncertainty intervals, and figures consistent with the published report.

**These bullets describe the documented analytic aims, not a specification sufficient to recreate every reported model.** In particular, do not invent covariate sets, impairment thresholds, missing-data rules, code for normative scoring, logistic reference categories, or coefficient values without the paper's full methods and original analysis scripts.

## Recommended next steps

1. Locate the original analysis directory or any older R/Rmd scripts, model logs, tables, and output files used for the 2025 article.
2. Recover the raw data dictionary and original script versions under appropriate restricted access. Do **not** commit datasets, participant-level output, credentials, or machine-specific paths to GitHub.
3. Compare models and output against the published article, including analytic sample sizes, cognitive composites, impairment definitions, adjustment sets, and follow-up cannabis-user-only analyses.
4. Preserve original syntax under a clearly labeled archival location (after privacy review). Create an independently executable, documented pipeline only after review and validation.
5. Once the neurocognition dissertation repository is manually renamed to `HIV.Cannabis.Neurocognition.2026`, update the related links across this repository, the ADL repository, and the academic website.

## Version control

This note was added without modifying existing scripts. Any newly synthesized code should be marked **reconstructed / not validated** until confirmed with the original data and article results. The published article remains the authoritative source.
