# Viscosity of water-lean CO2 absorbents

Data and simulation code for *Comparative Insights into Viscosity in Single-Component Water-Lean CO2 Absorbents*.

## Start here

Use the **[3 November 2026 data and code release](https://github.com/Nemo-ZJU-1998/Water-Lean-Absorbent-Viscosity/releases/tag/data-20261103-v2)** for the current manuscript sources.

| Download | Contents |
|---|---|
| [START_HERE.txt](https://github.com/Nemo-ZJU-1998/Water-Lean-Absorbent-Viscosity/releases/download/data-20261103-v2/START_HERE.txt) | Guide to the two packages and their scope. |
| [Source_Data_and_Analysis.zip](https://github.com/Nemo-ZJU-1998/Water-Lean-Absorbent-Viscosity/releases/download/data-20261103-v2/Source_Data_and_Analysis.zip) | Numerical results, figure and table inputs, analysis programs and simulation parameters. |
| [Simulation_Workflow_and_Example_Inputs.zip](https://github.com/Nemo-ZJU-1998/Water-Lean-Absorbent-Viscosity/releases/download/data-20261103-v2/Simulation_Workflow_and_Example_Inputs.zip) | Molecular preparation, GROMACS viscosity workflows, shared helpers and EEMPA example inputs. |
| [SHA256SUMS.txt](https://github.com/Nemo-ZJU-1998/Water-Lean-Absorbent-Viscosity/releases/download/data-20261103-v2/SHA256SUMS.txt) | Checksums for both ZIP archives. |
| [verification.json](https://github.com/Nemo-ZJU-1998/Water-Lean-Absorbent-Viscosity/releases/download/data-20261103-v2/verification.json) | Summary of file-integrity and numerical checks. |

Download these named assets rather than GitHub's automatically generated Source code archives.

## Find and verify a numerical result

Extract `Source_Data_and_Analysis.zip`. Read its `README.txt` and `FIGURE_DATA_INDEX.csv` to locate the inputs for a manuscript figure or table. Use the index inside this archive rather than the older index files in the repository root.

From the extracted directory, run:

```bash
python verify_archive.py
python verify_results.py
```

These commands verify file integrity and selected numerical results; they do not rerun molecular dynamics. The experimental comparison contains 49 pairs and has a mean absolute log10 error of **0.136**. Full numerical precision is retained in the data for recalculation. Missing uncertainty values remain missing. Other analysis programs require the inputs, dependencies and path configuration documented in the package.

## Use the simulation workflows

Extract `Simulation_Workflow_and_Example_Inputs.zip` and start with its `README.md`. The [online simulation guide](simulation/README.md) explains the program hierarchy, software dependencies, execution paths, scheduler settings and starting-state requirements. The shared-library and EEMPA example workflows have different settings; follow their documented variants. Generated per-loading jobs are produced by the supplied programs.

## Scope and raw trajectories

The packages provide data, analysis sources and simulation workflow examples. Complete starting inputs for all 16 systems are not included, and the packages are not a one-command reproduction of the entire paper. Raw trajectories are available from the corresponding authors upon reasonable request. Consult the data package documentation for remaining source limitations and the definitions of each analysis. Finite-window contact persistence should not be interpreted as a complete cluster lifetime.

## Earlier versions

[Previous releases](https://github.com/Nemo-ZJU-1998/Water-Lean-Absorbent-Viscosity/releases), including the 28 October data package and the preceding 3 November package, remain available for provenance. The scripts, numerical indexes, gap lists and checksums in the repository root belong to the **28 October 2026 version**. They are retained as historical files; the current download links and verification commands are those above. Earlier figure numbers and numerical summaries should not replace the current archive's figure-to-data mapping and results.

Third-party attribution and applicable terms are retained. This deposit does not grant a new licence to third-party material.
