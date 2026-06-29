<a id="readme-top"></a>

<div align="center">

# Yue Zhao (赵越)

**AI Risk Audit and Control across Agents, Foundation Models, and Data**

USC Professor · Founder of FORTIS Labs · Open-source author

[![Homepage](https://img.shields.io/badge/Homepage-USC-990000)](https://viterbi-web.usc.edu/~yzhao010/)
[![Google Scholar](https://img.shields.io/badge/Google%20Scholar-12k%2B%20citations-4285F4?logo=googlescholar&logoColor=white)](https://scholar.google.com/citations?user=zoGDYsoAAAAJ)
[![PyOD stars](https://img.shields.io/github/stars/yzhao062/pyod?style=flat&label=PyOD&color=990000)](https://github.com/yzhao062/pyod)
[![PyOD downloads](https://static.pepy.tech/badge/pyod)](https://pepy.tech/project/pyod)

[Homepage](https://viterbi-web.usc.edu/~yzhao010/) &nbsp;·&nbsp;
[Research](#research) &nbsp;·&nbsp;
[Open Source](#open-source) &nbsp;·&nbsp;
[FORTIS Lab](#fortis-lab) &nbsp;·&nbsp;
[Community](#community) &nbsp;·&nbsp;
[Contact](#contact)

</div>

> [!NOTE]
> Assistant Professor at USC Computer Science and PI of the **FORTIS Lab**. I research, build, and open-source **AI risk audit and control**: methods, benchmarks, and tools for inspecting and intervening on AI systems across the deployment stack. Creator of **PyOD**, the canonical Python anomaly-detection library (9.8k&#9733;; named by OpenAI, Apache Beam, PostHog, MLflow, and Genentech). Across my open source: **~24k GitHub stars and 42M+ downloads**. Co-authored work (TrustLLM) is cited in a **U.S. Senate HSGAC report, NIST AI 100-2e2025, and the International AI Safety Report 2026**. ~12k Google Scholar citations.

> [!IMPORTANT]
> **Founder of [FORTIS Labs](https://fortislabs.ai): a venture building auditable AI agents.** Open-source infrastructure to capture, verify, and roll back agent decisions, anchored by [`auditable`](https://github.com/yzhao062/auditable) and drawing on a decade of anomaly-detection research. Introductions from investors and design partners welcome at [hello@fortislabs.ai](mailto:hello@fortislabs.ai).

---

## Research

AI systems are deployed faster than they can be verified. Foundation models and autonomous agents now make consequential decisions, execute code, and interact with external services, often without systematic inspection of what they do or why. My research builds the methods, benchmarks, and open-source tools for **AI risk audit and control**.

Methodologically, this work extends my prior research on **anomaly and outlier detection** (the basis of the [PyOD](https://github.com/yzhao062/pyod) ecosystem) from data distributions to foundation-model behavior and agent decision traces, where unsafe, anomalous, or out-of-policy actions must be detected and reconstructed before and after deployment.

Three layers of the deployment stack:

- 🤖 **Agent Layer: Risk Audit and Runtime Control.** Auditability frameworks ([Auditable Agents](https://arxiv.org/abs/2604.05485), [`auditable`](https://github.com/yzhao062/auditable)), runtime control that intercepts tool calls before they fire ([Aegis](https://github.com/Justin0504/Aegis)), static over-privilege scanning ([agent-audit](https://github.com/HeadyZhang/agent-audit)), post-run failure localization in multi-agent systems ([GRADE](https://github.com/yzhao062/grade)), and agent-specific failure modes (over-privilege, cross-user contamination, the autonomy tax of defense training).
- 🧠 **Foundation-Model Layer: Trust and Robustness.** Jailbreak detection for vision-language models, causal analysis of hallucination, query-agnostic attacks on retrieval-augmented generation, and LLM-as-anomaly-detector benchmarks.
- 📊 **Data Layer: Anomaly and Out-of-Distribution Detection.** PyOD ecosystem, ADBench, automatic OOD detector selection, modality-specific OOD methods, and few-shot cross-domain OOD detection.

---

## Open Source

**~24k GitHub stars and 42M+ downloads across projects.** Featured below (full list on the [homepage](https://viterbi-web.usc.edu/~yzhao010/opensource.html)):

| Project | Layer | What It Does |
|---|---|---|
| [**PyOD**](https://github.com/yzhao062/pyod) | Data | Canonical anomaly detection: 60+ detectors across tabular, time-series, graph, and image data. (9.8k&#9733;) |
| [**auditable**](https://github.com/yzhao062/auditable) | Agent | System of record for AI-agent decisions: capture, replay against live state, roll back. |
| [**agent-audit**](https://github.com/HeadyZhang/agent-audit) | Agent | Static security and over-privilege scanner for AI-agent code. |
| [**anywhere-agents**](https://github.com/yzhao062/anywhere-agents) | Tooling | One config for Claude Code and Codex across every project and session. (171&#9733;) |
| [**agent-style**](https://github.com/yzhao062/agent-style) | Tooling | 21 writing rules loaded into AI agents at generation time. (432&#9733;) |

> [!TIP]
> **External adoption of PyOD.** Named by [OpenAI](https://openai.com/careers/technical-intelligence-analyst-san-francisco/) as expected operational tooling, shipped as a first-class ModelHandler in [Apache Beam](https://github.com/apache/beam/blob/master/sdks/python/apache_beam/ml/anomaly/detectors/pyod_adapter.py) (Apache Software Foundation), running the live-traffic alerting subsystem in [PostHog](https://github.com/PostHog/posthog/tree/master/posthog/tasks/alerts/detectors/pyod_detectors), the canonical anomaly-detection flavor in [MLflow](https://github.com/mlflow/mlflow/blob/master/docs/docs/classic-ml/community-model-flavors/index.mdx) community-flavor docs, and embedded in [Genentech (Roche)](https://github.com/Genentech/data-detective) drug-discovery validators. 5,493 public repositories and 139 packages depend on PyOD (May 2026 snapshot). The U.S. DoD CDAO lists PyOD; ESA OPS-SAT flies it for spacecraft anomaly detection.

<details>
<summary><b>Other Notable Projects</b></summary>

- [**PyGOD**](https://github.com/pygod-team/pygod) (1.5k&#9733;): graph outlier detection, sister project to PyOD.
- [**GRADE**](https://github.com/yzhao062/grade): typed two-layer graph of agent execution and dependency; localizes the faulting step in multi-agent runs.
- [**Aegis**](https://github.com/Justin0504/Aegis) (contributor): pre-execution firewall that gates each agent tool call.
- [**TrustLLM**](https://github.com/HowieHwong/TrustLLM) (625&#9733;, co-author): LLM trustworthiness benchmark cited by NIST AI 100-2e2025, the FLI AI Safety Index, U.S. Senate HSGAC, and DoD CDAO.
- [**AD-AGENT**](https://github.com/USC-FORTIS/AD-AGENT) (99&#9733;): LLM-driven multi-agent anomaly detection platform.
- [**ADBench**](https://github.com/Minqi824/ADBench) (1k&#9733;): NeurIPS 2022 official anomaly detection benchmark.
- [**Anomaly-Detection-Resources**](https://github.com/yzhao062/anomaly-detection-resources) (9.3k&#9733;): curated resource hub for anomaly detection.
- [**CS-Paper-Checklist**](https://github.com/yzhao062/cs-paper-checklist) (1.6k&#9733;): practical sanity checklist for CS paper writing.
- [**agent-config**](https://github.com/yzhao062/agent-config): personal working repo and canonical source for `anywhere-agents`.

</details>

---

## FORTIS Lab

I lead the [FORTIS Lab](https://viterbi-web.usc.edu/~yzhao010/lab.html) at USC, working on AI risk audit and control, anomaly detection, and trustworthy AI systems, with a team of PhD, master's, and undergraduate researchers.

---

## Community

Founder & Maintainer of **[博士栈 · CSPhD.org](https://csphd.org)**, a non-profit community for CS / AI / EE / Stats PhDs. Since 2022 it has grown to several thousand members and helped many land PhD positions, internships, and full-time roles, with a searchable board of 540+ PhD, RA, and postdoc openings.

---

## Contact

- 🌐 [Homepage](https://viterbi-web.usc.edu/~yzhao010/) · [Google Scholar](https://scholar.google.com/citations?user=zoGDYsoAAAAJ) · [LinkedIn](https://www.linkedin.com/in/yzhao062/)
- ✉️ `yue.z [AT] usc.edu`

<div align="center">

<sub><a href="#readme-top">↑ back to top</a></sub>

</div>
