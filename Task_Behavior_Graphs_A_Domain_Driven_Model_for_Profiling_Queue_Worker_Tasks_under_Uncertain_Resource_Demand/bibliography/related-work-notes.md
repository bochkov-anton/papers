# Related Work Notes

## Cluster resource management

### Borg
- Citation key: `verma2015borg`
- Use for: cluster management, admission control, resource-aware execution, over-commitment.
- Relevance: supports the background that large-scale systems manage tasks/jobs using resource-aware mechanisms.
- Limitation relative to this paper: does not primarily define a queue-worker task profiling model or task-class-specific behavior graph.

### Dominant Resource Fairness
- Citation key: `ghodsi2011drf`
- Use for: multi-resource allocation and dominant-resource thinking.
- Relevance: supports the claim that task load cannot be reduced to a single scalar.
- Limitation relative to this paper: allocation/fairness mechanism, not profiling model.

## Workload characterization

### Characterizing Task Usage Shapes in Google Compute Clusters
- Citation key: `zhang2011taskusage`
- Use for: task usage shapes, runtime resource consumption, workload characterization.
- Relevance: supports resource-demand profiles and usage-shape framing.
- Limitation: cluster-level trace characterization, not queue-worker instrumentation model.

### Heterogeneity and Dynamicity of Clouds at Scale
- Citation key: `reiss2012heterogeneity`
- Use for: heterogeneity and dynamicity in production cloud workloads.
- Relevance: supports conditional and variable workload behavior.
- Limitation: trace analysis, not a domain-driven task behavior graph model.

### Alibaba co-located workloads
- Citation key: `cheng2018alibaba`
- Use for: co-located workload heterogeneity, batch/online differences, production trace analysis.
- Relevance: supports the need for workload-specific interpretation and resource orchestration.
- Limitation: datacenter workload analysis, not queue-worker task profiling.

## Workload classification and interference

### Paragon
- Citation key: `delimitrou2013paragon`
- Use for: unknown workload classification, heterogeneity, interference.
- Relevance: supports task-class-aware profiling and context sensitivity.
- Limitation: scheduling/classification system, not a manifest-driven profiling model.

### Quasar
- Citation key: `delimitrou2014quasar`
- Use for: avoiding reliance on user-provided resource reservations, performance constraints, classification.
- Relevance: supports the argument that declared resources are insufficient.
- Limitation: cluster manager, not queue-worker task behavior graphs.

## Tail latency and stragglers

### The Tail at Scale
- Citation key: `dean2013tail`
- Use for: tail latency, rare performance episodes, large-scale variability.
- Relevance: supports entropy/tail-risk discussion.
- Limitation: service-level latency, not task profiling.

### MapReduce
- Citation key: `dean2004mapreduce`
- Use for: large-scale task execution and straggler mitigation.
- Relevance: historical example of variable task completion and backup/speculative execution.
- Limitation: batch processing framework, not general queue-worker profiling.

## Observability and tracing

### Dapper
- Citation key: `sigelman2010dapper`
- Use for: distributed tracing, low overhead, application-level transparency.
- Relevance: supports tracing as an observation mechanism.
- Limitation: tracing infrastructure, not a model for deciding which task features matter.

### OpenTelemetry Sampling
- Citation key: `opentelemetrySampling`
- Use for: sampling strategies and overhead control.
- Relevance: supports profiling policy selection.
- Limitation: instrumentation framework documentation, not workload model.

### OpenTelemetry Metrics Data Model
- Citation key: `opentelemetryMetricsDataModel`
- Use for: metrics data model and semantic telemetry.
- Relevance: supports metrics/signals/features discussion.
- Limitation: telemetry data model, not task behavior model.

### OpenTelemetry Performance
- Citation key: `opentelemetryPerformance`
- Use for: telemetry overhead and high-cardinality concerns.
- Relevance: supports profiling budget and cardinality policy.
- Limitation: operational guidance, not profiling theory.

## Workload entropy and burstiness

### Workload Classification for Efficient Auto-Scaling
- Citation key: `alieldin2013wac`
- Use for: autocorrelation, sample entropy, burstiness, periodicity.
- Relevance: supports entropy/predictability metrics.
- Limitation: auto-scaling classification, not queue-worker task behavior graphs.