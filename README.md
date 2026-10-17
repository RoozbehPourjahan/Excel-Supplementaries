# Supplementary Data: AI-Based Research Assistants

Supplementary data for the manuscript *AI-Based Research Assistants: A Task-Oriented Review of Capability, Risk and Ethical Governance in Scientific Research* (Section 3.6; Tables 2, 6a and 6b).

## Contents

| File | Description |
|---|---|
| `Supplementary_Data.xlsx` | Cell-level data for the intra-rater reliability check |
| `LICENSE` | MIT License |

The workbook has two sheets. `README` documents the sampling and scoring procedure, the column definitions and the raw-to-Final score mapping. `Data` has 88 rows, one per sampled tool–task cell.

## What the data are

The review scores 12 tools on 49 tasks (588 cells). To check intra-rater consistency, 88 cells (15%) were drawn at random, stratified by the ten task categories with proportional (Largest Remainder) allocation, and re-scored in a second pass without consulting the first-pass value.

Columns of the `Data` sheet:

| Column | Meaning |
|---|---|
| `ID` | Running number of the sampled cell (1–88) |
| `Task`, `Category`, `Tool` | The sampled tool–task cell |
| `Pass1_Final` | First-pass Final score (1–5) as recorded in the matrix |
| `Pass2_S`, `Pass2_C`, `Pass2_E`, `Pass2_V` | Second-pass sub-factors, each 0–2: design suitability, native capability, evidence strength, verification burden |
| `Pass2_Raw` | S + C + E + V (formula, 0–8) |
| `Pass2_Final` | Second-pass Final score (1–5) |

Raw-to-Final mapping: 0–1 → 1; 2–3 → 2; 4–5 → 3; 6–7 → 4; 8 → 5. Full definitions of the 0/1/2 anchors for each sub-factor are in the workbook's `README` sheet.

## What the data do not include

- The full 49 × 12 score matrix is not tabulated here. All 588 cells are determined by Table 4 (task-to-category assignment), Table 5 (category-level defaults) and Table 6 (22 documented exceptions) of the manuscript, through the assembly rule of Section 3.5.6.
- First-pass sub-factor values exist only for the documented exceptions. Of the 88 sampled cells, only IDs 25, 51 and 75 are exceptions, and their first-pass vectors are identical to the second-pass vectors in the `Data` sheet.
- The random seed used for sampling was not recorded. The sampled cells are listed in full in the `Data` sheet.

## Reproducing the reported statistics

- Agreement statistics (Section 3.6) use `Pass1_Final` and `Pass2_Final`.
- Table 2 (Spearman correlations) and Table 6a (weighting sensitivity) use `Pass2_S`, `Pass2_C`, `Pass2_E` and `Pass2_V`.
- Table 6b gives the distribution of these four columns.
- Bootstrap confidence intervals will differ slightly from the published values unless the resampling is identical.

## Limitations

Both passes were carried out by the same rater in the same session, so agreement reflects same-session consistency rather than test–retest reliability. The sample is stratified but small. See Sections 3.6 and 14 of the manuscript.

## License

Released under the MIT License; see `LICENSE`.

## Citation

If you use these data, please cite the manuscript:

> Pourjahan, R. (2026). AI-Based Research Assistants: A Task-Oriented Review of Capability, Risk and Ethical Governance in Scientific Research. Supplementary data: https://github.com/RoozbehPourjahan/Excel-Supplementaries

## Contact

Roozbeh Pourjahan, via the GitHub profile [RoozbehPourjahan](https://github.com/RoozbehPourjahan).
