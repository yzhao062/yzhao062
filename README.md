<a id="readme-top"></a>

<div align="center">

# Yue Zhao (赵越)

**Building auditable AI systems: detection, verification, control, and cost**

USC Assistant Professor · Founder of Auditable AI · Open-source author

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
> Assistant Professor at USC Computer Science, PI of the **FORTIS Lab**, and Associate Co-Director of the **USC Institute on Ethics and Trust in Computing** for 2026-2027. I research, build, and open-source the methods, benchmarks, and infrastructure that **make AI systems auditable**. Four questions carry that work: the data going in, the output coming out, the action taken, and the effort spent. Creator of **PyOD**, the canonical Python anomaly-detection library, named by OpenAI and used by Apache Beam, Amazon, Walmart, Databricks, and the European Space Agency. Across the projects I lead or co-author: **29k+ GitHub stars and 60M+ downloads** (August 2026), including PyOD, ADBench, TrustLLM, agent-audit, and Aegis. Author of over 80 peer-reviewed papers with ~12k Google Scholar citations. Co-authored work (TrustLLM) is cited in a **U.S. Senate HSGAC report, NIST AI 100-2e2025, and the International AI Safety Report 2026**.

> [!IMPORTANT]
> **Founder of [Auditable AI](https://auditable.run), the auditable layer for AI agents.** Open-source infrastructure to capture each agent decision, replay it against live state, and roll it back when it no longer holds. It is anchored by [`auditable`](https://github.com/yzhao062/auditable) and draws on a decade of anomaly-detection research. Introductions from investors and design partners welcome at [hello@auditable.run](mailto:hello@auditable.run).
>
> Also serving as Chief Scientific Advisor to [Figwork](https://www.figwork.ai/), an AI platform for early-career talent.

---

## Research

AI systems are deployed faster than they can be verified. Foundation models and autonomous agents now make consequential decisions, execute code, and interact with external services, often without systematic inspection of what they do or why. My research builds the methods, benchmarks, and open-source infrastructure that **make AI systems auditable**: detecting, diagnosing, and controlling departures from expected behavior, from anomalous data and foundation-model failures to consequential agent actions. That same record answers a fourth question: whether the work an agent did was necessary at all.

Methodologically, this work extends my prior research on **anomaly and outlier detection** (the basis of the [PyOD](https://github.com/yzhao062/pyod) ecosystem) from data distributions to foundation-model behavior and agent decision traces, where unsafe, anomalous, or out-of-policy actions must be detected and reconstructed before and after deployment.

The same four audit questions the [homepage](https://viterbi-web.usc.edu/~yzhao010/) states, listed here newest first:

- 🤖 **Auditing of Action: Auditability and Control of Agent Systems.** Auditability frameworks ([Auditable Agents](https://arxiv.org/abs/2604.05485), [`auditable`](https://github.com/yzhao062/auditable)), runtime control that intercepts tool calls before they fire ([Aegis](https://github.com/Justin0504/Aegis)), and static over-privilege scanning ([agent-audit](https://github.com/HeadyZhang/agent-audit)) with its benchmark ([FORTIS](https://arxiv.org/abs/2605.09163)). Also post-run failure localization in multi-agent systems ([GRADE](https://arxiv.org/abs/2606.22741)) and agent-specific failure modes: over-privilege and cross-user contamination.
- ⚡ **Optimization of Effort: Agent Efficiency, Routing, and the Cost of Defense.** Whether the work an agent did was necessary, read from the same record that makes it accountable, and the dimension industry asks about most. [The Autonomy Tax](https://arxiv.org/abs/2603.19423) measures what defense training against prompt injection costs an agent's ability to finish multi-step tasks. [Bandit routing](https://arxiv.org/abs/2510.07429) treats model choice as an online cost-quality decision, and [DyFlow](https://openreview.net/forum?id=0pbUfmwNTy) constructs agent workflows as a run proceeds. The question runs back through the detection line, where [SUOD](https://proceedings.mlsys.org/paper_files/paper/2021/hash/37385144cac01dff38247ab11c119e3c-Abstract.html) and the GPU-accelerated [TOD](https://www.vldb.org/pvldb/vol16/p546-zhao.pdf) cut the compute cost of running many detectors at scale.
- 🧠 **Verification of Output: Trust and Robustness of Foundation Models.** Jailbreak detection for vision-language models, causal analysis of hallucination, query-agnostic attacks on retrieval-augmented generation, and LLM-as-anomaly-detector benchmarks.
- 📊 **Detection in Data: Anomaly and Out-of-Distribution Detection.** PyOD ecosystem, ADBench, automatic OOD detector selection, modality-specific OOD methods, and few-shot cross-domain OOD detection.

Our position paper [Auditable Agents](https://arxiv.org/abs/2604.05485) organizes this into five dimensions of auditability and three mechanism classes (detect, enforce, recover). It appears at the inaugural ACM AI Leadership Summit and at the ACL 2026 KnowFM workshop.

---

## Open Source

**29k+ GitHub stars and 60M+ downloads across the projects I lead or co-author** (August 2026). Featured below (full list on the [homepage](https://viterbi-web.usc.edu/~yzhao010/opensource.html)):

| Project | Audit question / role | Stars | What It Does |
|---|---|---|---|
| [**PyOD**](https://github.com/yzhao062/pyod) | Detection in data | [![PyOD GitHub stars](https://img.shields.io/github/stars/yzhao062/pyod?style=flat&label=%20&color=990000)](https://github.com/yzhao062/pyod) | Canonical anomaly detection, now in its third major release. 60+ detectors across tabular, time series, graph, text, and image data, plus an ADEngine orchestration core and an agentic investigation layer driven in natural language. |
| [**auditable**](https://github.com/yzhao062/auditable) | Auditing of action | [![auditable GitHub stars](https://img.shields.io/github/stars/yzhao062/auditable?style=flat&label=%20&color=990000)](https://github.com/yzhao062/auditable) | System of record for AI-agent decisions: capture, replay against live state, roll back. |
| [**GRADE**](https://github.com/yzhao062/grade) | Auditing of action | [![GRADE GitHub stars](https://img.shields.io/github/stars/yzhao062/grade?style=flat&label=%20&color=990000)](https://github.com/yzhao062/grade) | The method `auditable` is built on: a typed two-layer graph of agent execution and dependency. [arXiv](https://arxiv.org/abs/2606.22741) |
| [**agent-audit**](https://github.com/HeadyZhang/agent-audit) | Auditing of action | [![agent-audit GitHub stars](https://img.shields.io/github/stars/HeadyZhang/agent-audit?style=flat&label=%20&color=990000)](https://github.com/HeadyZhang/agent-audit) | Static security and over-privilege scanner for AI-agent code. |
| [**awesome-auditable-ai**](https://github.com/yzhao062/awesome-auditable-ai) | Auditing of action | [![awesome-auditable-ai GitHub stars](https://img.shields.io/github/stars/yzhao062/awesome-auditable-ai?style=flat&label=%20&color=990000)](https://github.com/yzhao062/awesome-auditable-ai) | Curated map of papers, tools, datasets, and standards for reliable, auditable AI agents. |
| [**anywhere-agents**](https://github.com/yzhao062/anywhere-agents) | Supporting tooling | [![anywhere-agents GitHub stars](https://img.shields.io/github/stars/yzhao062/anywhere-agents?style=flat&label=%20&color=990000)](https://github.com/yzhao062/anywhere-agents) | One config for Claude Code and Codex across every project and session. |
| [**agent-style**](https://github.com/yzhao062/agent-style) | Supporting tooling | [![agent-style GitHub stars](https://img.shields.io/github/stars/yzhao062/agent-style?style=flat&label=%20&color=990000)](https://github.com/yzhao062/agent-style) | 21 writing rules loaded into AI agents at generation time. |

> [!TIP]
> **External adoption of PyOD.** Named by [OpenAI](https://openai.com/careers/technical-intelligence-analyst-san-francisco/) as expected operational tooling, shipped as a first-class ModelHandler in [Apache Beam](https://github.com/apache/beam/blob/master/sdks/python/apache_beam/ml/anomaly/detectors/pyod_adapter.py) (Apache Software Foundation), running the live-traffic alerting subsystem in [PostHog](https://github.com/PostHog/posthog/tree/master/posthog/tasks/alerts/detectors/pyod_detectors), the canonical anomaly-detection flavor in [MLflow](https://github.com/mlflow/mlflow/blob/master/docs/docs/classic-ml/community-model-flavors/index.mdx) community-flavor docs, and embedded in [Genentech (Roche)](https://github.com/Genentech/data-detective) drug-discovery validators. It is also used by Amazon, Walmart, and Databricks, runs inside published procurement audits by the Brazilian federal government, and is deployed in a UK Government care service. 5,493 public repositories and 139 packages depend on PyOD (May 2026 snapshot). The U.S. DoD CDAO lists PyOD; ESA OPS-SAT flies it for spacecraft anomaly detection. PyOD is the subject of five published books and is cited in 49 patents.

<details>
<summary><b>Other Notable Projects</b></summary>

- [**PyGOD**](https://github.com/pygod-team/pygod) [![PyGOD GitHub stars](https://img.shields.io/github/stars/pygod-team/pygod?style=flat&label=%20&color=990000)](https://github.com/pygod-team/pygod): graph outlier detection, sister project to PyOD.
- [**Aegis**](https://github.com/Justin0504/Aegis) [![Aegis GitHub stars](https://img.shields.io/github/stars/Justin0504/Aegis?style=flat&label=%20&color=990000)](https://github.com/Justin0504/Aegis) (contributor): pre-execution firewall that gates each agent tool call.
- [**TrustLLM**](https://github.com/HowieHwong/TrustLLM) [![TrustLLM GitHub stars](https://img.shields.io/github/stars/HowieHwong/TrustLLM?style=flat&label=%20&color=990000)](https://github.com/HowieHwong/TrustLLM) (co-author): LLM trustworthiness benchmark cited by NIST AI 100-2e2025, the FLI AI Safety Index, U.S. Senate HSGAC, and DoD CDAO.
- [**Therapeutics Data Commons**](https://github.com/mims-harvard/TDC) [![Therapeutics Data Commons GitHub stars](https://img.shields.io/github/stars/mims-harvard/TDC?style=flat&label=%20&color=990000)](https://github.com/mims-harvard/TDC) (co-author): supplied the training data for Google Research's Tx-LLM and the prediction tasks in Google DeepMind's TxGemma.
- [**AD-AGENT**](https://github.com/USC-FORTIS/AD-AGENT) [![AD-AGENT GitHub stars](https://img.shields.io/github/stars/USC-FORTIS/AD-AGENT?style=flat&label=%20&color=990000)](https://github.com/USC-FORTIS/AD-AGENT): LLM-driven multi-agent anomaly detection platform.
- [**ADBench**](https://github.com/Minqi824/ADBench) [![ADBench GitHub stars](https://img.shields.io/github/stars/Minqi824/ADBench?style=flat&label=%20&color=990000)](https://github.com/Minqi824/ADBench): NeurIPS 2022 official anomaly detection benchmark.
- [**Anomaly-Detection-Resources**](https://github.com/yzhao062/anomaly-detection-resources) [![Anomaly-Detection-Resources GitHub stars](https://img.shields.io/github/stars/yzhao062/anomaly-detection-resources?style=flat&label=%20&color=990000)](https://github.com/yzhao062/anomaly-detection-resources): curated resource hub for anomaly detection.
- [**CS-Paper-Checklist**](https://github.com/yzhao062/cs-paper-checklist) [![CS-Paper-Checklist GitHub stars](https://img.shields.io/github/stars/yzhao062/cs-paper-checklist?style=flat&label=%20&color=990000)](https://github.com/yzhao062/cs-paper-checklist): practical sanity checklist for CS paper writing.
- [**agent-config**](https://github.com/yzhao062/agent-config): personal working repo and canonical source for `anywhere-agents`.

</details>

---

## FORTIS Lab

I lead the [FORTIS Lab](https://viterbi-web.usc.edu/~yzhao010/lab.html) at USC, working on auditable AI systems, anomaly detection, and foundation-model trust, with a team of PhD, master's, and undergraduate researchers.

My awards include the NVIDIA Academic Grant Program Award, multiple Amazon Research Awards, the Capital One Research Award, and the Foresight Institute AI for Safety & Science Nodes Grant. NSF grants and a Meta sponsored research agreement fund the lab alongside them. AAAI selected me for New Faculty Highlights.

---

## Community

Founder & Maintainer of **[博士栈 · CSPhD.org](https://csphd.org)**, a non-profit community for CS / AI / EE / Stats PhDs. Since 2022 it has grown to several thousand members and helped many land PhD positions, internships, and full-time roles, with a searchable board of 500+ PhD, RA, and postdoc openings.

---

## Contact

- 🌐 [Homepage](https://viterbi-web.usc.edu/~yzhao010/) · [Google Scholar](https://scholar.google.com/citations?user=zoGDYsoAAAAJ) · [LinkedIn](https://www.linkedin.com/in/yzhao062/)
- ✉️ `yue.z [AT] usc.edu`

<div align="center">

<sub><a href="#readme-top">↑ back to top</a></sub>

</div>
