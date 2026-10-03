# M Talha

### AI Security Engineer at Cytomate · AI Red Teaming · AI Security Solutions

I find the ways AI systems break, and I build the defences that make them harder to break. My background is penetration testing. Today I work on **AI red teaming** and on **AI security products**, and I do research on **LLM and machine-learning security** in my own time.

📍 Islamabad, Pakistan · 🌐 [odynsec.com](https://odynsec.com) · ✉️ m.talha@cytomate.net

---

## What I work on

| | |
|---|---|
| **AI red teaming** | Attacking LLM and RAG systems the way a real adversary would: prompt injection, secret extraction, agentic and retrieval-layer exploits. |
| **AI security solutions** | Building detection, filtering and triage tools that put LLMs and machine learning to work for defenders. |
| **Evaluation you can trust** | Leak-free splits, honest baselines, and a written account of what a result does *not* show. |

---

## Featured work

### Attack and defence of RAG systems

| Project | What it is | Headline result |
|---|---|---|
| [**MemLeak-RL**](https://github.com/xorai-sec/MemLeak-RL-Deep-RL-Red-Agent-for-RAG-System-Exploitation) | A red-team agent that learns, through supervised fine-tuning and PPO, to extract secrets from RAG systems by abusing the retriever's *confused-deputy* behaviour. LLaMA-3-8B + QLoRA + FAISS. | **84.2%** attack success on GPT-Neo-2.7B, **98.0%** on Phi-3-Mini, **71.4%** against a Llama-Guard-2 victim. |
| [**RAG-Sentinel**](https://github.com/xorai-sec/rag-sentinel) | A lightweight filter that screens retrieved passages for hidden instructions before they reach the LLM. | Attack success **35.4% → 1.0%** in simulation, and an audit that exposes a dataset shortcut so the scores are not over-claimed. |

### LLMs and machine learning for security operations

| Project | What it is | Headline result |
|---|---|---|
| [**MCASM**](https://github.com/xorai-sec/mcasm-multicloud-attack-surface-slm) | A QLoRA-tuned 3B model that triages findings across AWS, Azure and GCP. | Kendall τ-b **0.745** vs 0.066 untrained. Matches a hand-built rule system on expert agreement (0.848 vs 0.800, not significant) and adds explanations. |
| [**Explainable Malware Detection**](https://github.com/xorai-sec/explainable-malware-detection) | Measures whether SHAP and LIME explanations can be trusted, on PDF and Android malware. | Accurate and faithful (0.92), but **unstable (0.44)** and inconsistent between methods (0.15). |

### Do security ML results survive contact with reality?

| Project | What it is | Headline result |
|---|---|---|
| [**NIDS Benchmark Reality Check**](https://github.com/xorai-sec/nids-benchmark-reality-check) | One leak-free pipeline over three intrusion-detection benchmarks. | In-dataset PR-AUC 0.99996 falls to **0.07–0.24** across datasets. |
| [**NIDS PCAP Deployment Gap**](https://github.com/xorai-sec/nids-pcap-deployment-gap) | Benchmark-trained models tested on independently extracted traffic. | 99.9% on the benchmark; a Random Forest flagged none of 3,978 malicious flows. |
| [**Federated DP-IDS**](https://github.com/xorai-sec/federated-dp-ids) | Federated learning with differential privacy for intrusion detection. | Federation is free (F1 0.9947 vs 0.9944). ε = 1 costs about 1.3 points. |

---

## How I work

- **Break it first.** I start from the attacker's view, then build the defence.
- **Measure honestly.** Every project reports its limits, such as dataset shortcuts, small expert studies and approximate extractors.
- **Make it reproducible.** Pinned sources, saved outputs, and notebooks that run end to end.

## Toolbox

**Offensive:** AI red teaming · prompt injection · RAG exploitation · penetration testing
**Models:** PyTorch · Hugging Face Transformers / PEFT (QLoRA) · PPO / reinforcement learning · scikit-learn · XGBoost / LightGBM
**Defence and trust:** SHAP / LIME · differential privacy (Opacus) · federated learning · FAISS · Scapy · Streamlit

---

I am open to research collaboration and research-assistant opportunities in **AI security, LLM red teaming and trustworthy ML for cyber defence**. The quickest way to reach me is m.talha@cytomate.net.

*My offensive-security work is for research and for systems I am authorised to test.*
