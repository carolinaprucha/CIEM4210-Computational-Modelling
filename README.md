# CIEM4210 Project Report Template

LaTeX template for **CIEM4210: Computational Modelling**.

The template is tailored to the course project on modelling a floating offshore wind turbine (OC3 Phase-IV spar-buoy) and focuses on the numerical modelling workflow using the Finite Element Method.

## Deliverables Covered by This Template

- Report (maximum **15 pages** excluding appendices)
- Executable script or notebook for reproducibility

## Submission Deadline

**Friday 12 June 2026 at 17:00** via Brightspace Assignments.

## Repository Structure

- `main.tex`: main report entry point
- `style.tex`: formatting and reusable placeholder commands
- `chapters/01_model_definition.tex`
- `chapters/02_numerical_methods.tex`
- `chapters/03_numerical_schemes.tex`
- `chapters/04_results_analysis.tex`

## Build

```bash
latexmk -pdf main.tex
```

Clean auxiliary files:

```bash
latexmk -c
```

## Report Logic

1. Model Definition
2. Numerical Discretization (FEM)
3. Numerical Schemes and Implementation
4. Numerical Verification and Results Interpretation

## Core + Choice Architecture

- Core Model (mandatory): 2D FOWT structural representation (RNA point mass, thin-beam tower, rigid-body spar-buoy, spring/damper mooring), baseline Airy-wave/Morison/thrust/current loading, FEM discretization, dynamic response assessment, and reduced-order/modal extension.
- Choice Packages (for maximum grade): coupled axial-bending tower model, geometrically nonlinear mooring strings, flexible-beam floater representation, irregular-wave loading, time-dependent thrust force, and/or time-dependent current force.

## Section Boundary Rules

- Section 1: assumptions, scope limits, and continuous model definition.
- Section 2: discrete FEM formulation and discretization choices only.
- Section 3: implementation and algorithmic design choices.
- Section 4: verification first (convergence/stability/modal), then interpreted engineering results.

## Assessment Criteria

| Criterion | Points |
|---|---|
| Quality of the final model | 10 |
| Correct definition and derivation of numerical model | 30 |
| Correct implementation of numerical model | 10 |
| Correct analysis of results (convergence, validation, response) | 50 |
| **Total** | **100** |

## Suggested Milestones

1. Week 1–2: One-page scope proposal (Core + selected Choice Packages).
2. Week 3: Model definition freeze (assumptions and equations).
3. Week 4–5: Discretization and implementation checkpoint.
4. Week 6: Verification checkpoint (convergence and stability evidence).
5. Final week: Results interpretation and report consolidation.

## Notes

- Replace all instructional placeholders before submission.
- Keep derivation details and long code excerpts in appendices.
- Provide explicit validation, convergence checks, and literature comparison.
- If AI is used, complete the in-depth acknowledgement in main.tex.
