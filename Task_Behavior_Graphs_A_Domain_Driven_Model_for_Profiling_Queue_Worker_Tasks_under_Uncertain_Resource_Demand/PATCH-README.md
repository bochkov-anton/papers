# Formal logic refactor patch

This patch resolves the current formal-model problems in the early sections.

Included files:

- sections/01-introduction.tex
- sections/02-terminology-and-notation.tex
- sections/03-background-and-motivation.tex
- sections/04-problem-statement.tex
- sections/05-task-cost-model.tex
- tables/terminology/12-notation.tex
- tables/terminology/core-terms.tex

Main changes:

1. Cost dimensions are now typed descriptors, not metric names.
   Each dimension q has:
   - role rho_q
   - unit u_q
   - value domain V_q
   - attribution boundary alpha_q
   - observation semantics omega_q
   - composition semantics kappa_q

2. The universal formula baseline * amplification + overhead is no longer
   treated as the only cost law. It is now a common affine specialization.
   The general model uses dimension-specific estimators and dimension-specific
   composition semantics.

3. Task-kind model state theta_k is introduced.
   This links history, calibration, declared descriptors, residual statistics,
   quantile sketches, and domain rules to the actual cost estimator.

4. z_a, x_a, and c_a are formalized:
   - z_a is the canonical feature vector.
   - x_a = P_X(z_a) is the intrinsic-feature projection.
   - c_a = P_C(z_a) is the execution-context projection.

5. Observed values are clarified:
   - Y_q(a) is not raw telemetry.
   - It is an attempt-attributed observed value according to omega_q.
   - residual epsilon_q(a) exists only when Y_q(a) exists.

6. Resource demand and worker occupancy are separated more strictly:
   - resource demand is modeled expected active resource need;
   - resource usage is observed attempt-attributed resource use;
   - worker occupancy is capacity held during explicit intervals.

7. Problem Statement now separates output classes:
   - cost estimates;
   - reliability diagnostics;
   - risk interpretation;
   - profiling-policy recommendation.
