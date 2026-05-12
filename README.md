<a id="readme-top"></a>

<div align="center">

# Yue Zhao (赵越)

**USC Assistant Professor building methods, benchmarks, and open-source tools for AI auditing.**

[![Homepage](https://img.shields.io/badge/Homepage-USC-990000)](https://viterbi-web.usc.edu/~yzhao010/)
[![Google Scholar](https://img.shields.io/badge/Google%20Scholar-12k%2B%20citations-4285F4?logo=googlescholar&logoColor=white)](https://scholar.google.com/citations?user=zoGDYsoAAAAJ)
[![PyOD stars](https://img.shields.io/github/stars/yzhao062/pyod?style=flat&label=PyOD&color=990000)](https://github.com/yzhao062/pyod)
[![PyOD downloads](https://static.pepy.tech/badge/pyod)](https://pepy.tech/project/pyod)

[Homepage](https://viterbi-web.usc.edu/~yzhao010/) &nbsp;·&nbsp;
[Research](#research) &nbsp;·&nbsp;
[Open Source](#open-source) &nbsp;·&nbsp;
[FORTIS Lab](#fortis-lab) &nbsp;·&nbsp;
[Contact](#contact)

</div>

> [!NOTE]
> Assistant Professor at USC Computer Science, PI of FORTIS Lab. Research on AI auditing: methods, benchmarks, and open-source tools for inspecting AI systems. Lead developer of PyOD (9.8k★, 42M+ downloads), the canonical Python anomaly-detection library, named by OpenAI, Apache Beam, PostHog, MLflow, and Genentech. ~12k Google Scholar citations across all work.

---

## Research

AI systems are deployed faster than they can be verified. Foundation models and autonomous agents now make consequential decisions, execute code, and interact with external services, often without systematic inspection of what they do or why. My research builds the methods, benchmarks, and open-source tools for **AI auditing**.

Methodologically, this work extends my prior research on **anomaly and outlier detection** (the basis of the [PyOD](https://github.com/yzhao062/pyod) ecosystem) from data-distribution settings to foundation-model behavior and autonomous-agent decision traces, where unsafe, anomalous, or out-of-policy actions must be detected and reconstructed before deployment.

Three connected directions:

- 🔍 **Auditing and Assurance:** methods, benchmarks, and tools to inspect and evaluate AI systems.
- 🛡️ **Safety and Security:** failure modes, attack surfaces, runtime guardrails.
- 🌐 **Science and Society:** AI for climate, healthcare, and computational social systems where accountability is not optional.

---

## Open Source

Featured projects (see the full list on the [homepage](https://viterbi-web.usc.edu/~yzhao010/opensource.html)):

| Project | What It Does |
|---|---|
| [**agent-style**](https://github.com/yzhao062/agent-style) | 21 writing rules for AI agents, loaded at generation time. (432★) |
| [**anywhere-agents**](https://github.com/yzhao062/anywhere-agents) | One config for Claude Code and Codex across every project and session. (171★) |
| [**agent-audit**](https://github.com/HeadyZhang/agent-audit) | OWASP Agentic Top 10 checks, taint analysis, and MCP auditing. (168★) |
| [**Aegis**](https://github.com/Justin0504/Aegis) | Pre-execution policy firewall for AI agents with audit trails. (353★) |
| [**PyOD**](https://github.com/yzhao062/pyod) | Agentic anomaly detection: 60+ detectors, 42M+ downloads. (9.8k★) |

> [!TIP]
> **External adoption of PyOD.** Named by [OpenAI](https://openai.com/careers/technical-intelligence-analyst-san-francisco/) as expected operational tooling, shipped as a first-class ModelHandler in [Apache Beam](https://github.com/apache/beam/blob/master/sdks/python/apache_beam/ml/anomaly/detectors/pyod_adapter.py) (Apache Software Foundation), running the live-traffic alerting subsystem in [PostHog](https://github.com/PostHog/posthog/tree/master/posthog/tasks/alerts/detectors/pyod_detectors), the canonical anomaly-detection flavor in [MLflow](https://github.com/mlflow/mlflow/blob/master/docs/docs/classic-ml/community-model-flavors/index.mdx) community-flavor docs, and embedded in [Genentech (Roche)](https://github.com/Genentech/data-detective) drug-discovery validators. 5,493 public repositories and 139 packages depend on PyOD (May 2026 snapshot). DoD CDAO lists PyOD and TrustLLM; ESA OPS-SAT uses PyOD; NIST AI 100-2e2025 and the FLI AI Safety Index cite TrustLLM.

<details>
<summary><b>Other Notable Projects</b></summary>

- [**PyGOD**](https://github.com/pygod-team/pygod) (1.5k★): graph outlier detection, sister project to PyOD.
- [**AD-AGENT**](https://github.com/USC-FORTIS/AD-AGENT) (99★): LLM-driven multi-agent anomaly detection platform.
- [**ADBench**](https://github.com/Minqi824/ADBench) (1k★): NeurIPS 2022 official anomaly detection benchmark.
- [**Anomaly-Detection-Resources**](https://github.com/yzhao062/anomaly-detection-resources) (9.3k★): curated resource hub for anomaly detection.
- [**CS-Paper-Checklist**](https://github.com/yzhao062/cs-paper-checklist) (1.6k★): practical sanity checklist for CS paper writing.
- [**TrustLLM**](https://github.com/HowieHwong/TrustLLM) (625★, collaborator): LLM trustworthiness benchmark cited by NIST AI 100-2e2025, FLI AI Safety Index, U.S. Senate HSGAC, DoD CDAO.
- [**agent-config**](https://github.com/yzhao062/agent-config): personal working repo and canonical source for `anywhere-agents`.

</details>

---

## FORTIS Lab

I lead the [FORTIS Lab](https://viterbi-web.usc.edu/~yzhao010/lab.html) at USC, working on AI auditing, anomaly detection, and trustworthy AI systems. Current roster: 4 PhD students plus master and undergraduate researchers.

---

## Contact

- 🌐 [Homepage](https://viterbi-web.usc.edu/~yzhao010/) · [Google Scholar](https://scholar.google.com/citations?user=zoGDYsoAAAAJ) · [LinkedIn](https://www.linkedin.com/in/yzhao062/)
- ✉️ `yue.z [AT] usc.edu`

<div align="center">

<sub><a href="#readme-top">↑ back to top</a></sub>

</div>
