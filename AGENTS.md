# Agent Notes for spiffe

This file contains a short tactical summary based on repository evidence. `../llm-wiki/scripts/refresh_wiki.py` rewrites only the machine-managed block.

<!-- BEGIN MACHINE:summary -->
## Quick start
- Repository-local guidance is sufficient: start with `AGENTS.md`, `README.md`, `docs/`, build/test/config files, and the source tree.
- **spiffe** is a 2.5-dimensional particle-in-cell (PIC) code developed at the Advanced Photon Source (APS) for the design and simulation of radio-frequency (RF) guns. This software is tailored to model the behavior of charged particles under the influence of electromagnetic fields, with a particular focus on the dynamics within RF guns. **spiffe** generates particle output files in the SDDS (Self-Describing Data Sets) format, which can be directly read and analyzed by the **elegant** software for downstream beamline simulations and analysis.
- Primary work areas: `documentation`, `examples`, `rpm`, `src`.

## Read first
- `README.md`: Primary project overview and workflow notes
- `documentation/Makefile`: Build system entry point or dependency manifest
- `src/Makefile`: Build system entry point or dependency manifest
- `LICENSE`: Repository configuration that affects local work
- `src/spiffe.c`: Source file named after the repository

## Build and test
- Detected build systems: GNU Make.
- Unknown: no test workflow evidence was found in the inspected files.
- Likely run commands or operator entry points: `./spiffe`.

## Operational warnings
- Local checkout layout appears significant; avoid casual changes to sibling-repo assumptions or relative paths.
- Platform-specific dependency setup matters; do not assume one platform's build recipe carries over unchanged.

## Compatibility constraints
- Cross-platform support exists, but platform-specific dependency setup matters.
- Build and runtime behavior likely depends on neighboring core toolkit checkouts.

## Related knowledge
- Repository-local documentation should be treated as authoritative.
- If a shared `llm-wiki/` directory is present in this workspace or parent folder, consult [the matching repo page](../llm-wiki/repos/spiffe.md) for additional architectural context.
- If no shared wiki is present, continue using repository-local evidence only.
- If available, [the SDDS concept page](../llm-wiki/concepts/sdds.md) adds broader cross-repo context.
- If present in this workspace, [the cross-repo map](../llm-wiki/insights/cross-repo-map.md) helps explain related repositories.
<!-- END MACHINE:summary -->

## Human notes
Add durable repo-specific instructions here.
