# Structural refactor patch

This patch restructures the implemented early paper sections and notation.

Included files:

- sections/01-introduction.tex
- sections/02-terminology-and-notation.tex
- sections/03-background-and-motivation.tex
- sections/04-problem-statement.tex
- sections/05-task-cost-model.tex
- tables/terminology/12-notation.tex

Main goals:

1. Make each section responsible for one role:
   - 01: motivation, claim, contributions, roadmap.
   - 02: compact terminology and notation.
   - 03: explanatory background and role distinctions.
   - 04: formal problem statement.
   - 05: formal cost model.

2. Remove repeated explanations across 01-05.

3. Fix the formal inconsistency where cost included "overhead" as if it were a
   third output family. The cost object now has two output families:
   resource demand and worker occupancy. Overhead contributes to dimensions.

4. Fix notation that mixed observed usage and estimated demand.

5. Make z_a, x_a, and c_a consistent:
   - z_a is the canonical feature vector.
   - x_a is the intrinsic-feature projection.
   - c_a is the execution-context projection.

6. Add dimension-generic cost notation:
   - Q = R union O.
   - Y_hat_q(a) is estimated value for a cost dimension.
   - Y_q(a) is observed attempt-attributed value when available.
   - epsilon_q(a) is residual.

Apply by copying this archive contents over the paper root.
