# Task Behavior Graphs terminology and appendix patch

This patch reorganizes the terminology structure of the paper.

## Main changes

- `sections/02-terminology-and-notation.tex` now contains only core terminology and notation.
- `tables/terminology/core-terms.tex` adds a compact core-term table for the main body.
- `appendices/a-extended-terminology.tex` adds a full extended glossary appendix.
- `main.tex` now includes the extended terminology appendix before taxonomy/schema appendices.
- Appendix placeholders are renamed in the input order so appendix letters remain meaningful:
  - `a-extended-terminology`
  - `b-extended-taxonomy`
  - `c-manifest-schema`
  - `d-algorithm-details`
  - `e-case-study-details`
  - `f-evaluation-methodology`
  - `g-reproducibility-checklist`
- Terminology tables were corrected:
  - `dependency wait time` is no longer treated as active resource demand.
  - `behavior` / `task behavior` duplication was removed.
  - `semantic feature` is now explicitly an informal alias; `canonical feature` remains preferred.
  - `acknowledge` and `ack` were merged into one glossary row.

## Apply

Copy the contents of this archive over the root paper directory:

`Task_Behavior_Graphs_A_Domain_Driven_Model_for_Profiling_Queue_Worker_Tasks_under_Uncertain_Resource_Demand/`

Old unused appendix files may remain in the repository, but `main.tex` no longer imports the old appendix order.
