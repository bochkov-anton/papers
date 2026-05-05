# Compile-safe core refactor patch

This patch fixes the LaTeX errors reported in the compile log and completes the
core paper spine.

Key fixes:

1. Replaced unsafe raw backtick identifiers with LaTeX-safe \texttt{...} forms.
2. Fixed the descriptor mismatch: u_q is used consistently.
3. Made cost vectors contain estimate objects rather than only point estimates.
4. Added/updated sections 05-20 with compile-safe content.
5. Added abstract, notation, core terms, manifest example, and claims/evidence map.

The compile log showed Missing $ errors caused by identifiers with underscores
inside backticks. This patch removes those blockers in sections 08 and 14 and
prevents the cascading errors in sections 09 and 15.
