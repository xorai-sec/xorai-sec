# M Talha

**AI Security Researcher · AI Red Teamer** · AI Security Engineer at Cytomate

I test how AI systems fail under attack, and I build the tools and evidence that make them safer to deploy. Background in penetration testing, now focused on LLM, RAG and ML security.

[odynsec.com](https://odynsec.com) · m.talha@cytomate.net · Islamabad

---

## At Cytomate: AEVA

**AEVA** is an open platform for AI assurance. It red-teams an AI system and turns the results into audit-ready evidence.

- **Red-team assessment** across four engines (garak, PyRIT, promptfoo and a native canary-based engine)
- **Replayable evidence**: every finding is tied to a hashed prompt and response
- **Compliance mapping** to NIST AI RMF, OWASP LLM Top 10, MITRE ATLAS, ISO/IEC 42001 and the EU AI Act
- **CI/CD ready**: `aeva gate` fails a build when an assessment fails

---

## Research and open-source work

**Attacking and defending RAG / LLM systems**

| | |
|---|---|
| [**MemLeak-RL**](https://github.com/xorai-sec/MemLeak-RL-Deep-RL-Red-Agent-for-RAG-System-Exploitation) | A reinforcement-learning red-team agent that extracts secrets from RAG systems. **84.2%** attack success on GPT-Neo-2.7B, **98.0%** on Phi-3-Mini. |
| [**RAG-Sentinel**](https://github.com/xorai-sec/rag-sentinel) | A filter that blocks hidden instructions in retrieved text. Attack success **35.4% → 1.0%**, plus an audit of dataset shortcuts. |

**AI for security operations**

| | |
|---|---|
| [**MCASM**](https://github.com/xorai-sec/mcasm-multicloud-attack-surface-slm) | A small LLM fine-tuned to prioritise multi-cloud security findings. Matches a rule system on expert agreement and adds explanations. |
| [**Explainable Malware Detection**](https://github.com/xorai-sec/explainable-malware-detection) | Measures whether SHAP and LIME explanations can be trusted. They turn out to be accurate but unstable. |

**Do security ML results hold up outside the benchmark?**

| | |
|---|---|
| [**NIDS Benchmark Reality Check**](https://github.com/xorai-sec/nids-benchmark-reality-check) | A 99.99% benchmark score falls to **7–24%** on a different network. |
| [**NIDS PCAP Deployment Gap**](https://github.com/xorai-sec/nids-pcap-deployment-gap) | 99.9% on the benchmark, yet a Random Forest flagged none of 3,978 malicious flows on raw PCAP. |
| [**Federated DP-IDS**](https://github.com/xorai-sec/federated-dp-ids) | Federated learning with differential privacy: federation costs nothing, and ε = 1 costs about 1.3 points. |

---

**Focus:** AI red teaming · LLM and RAG security · prompt injection · AI assurance · trustworthy ML for cyber defence

**Tools:** Python · PyTorch · Hugging Face · PEFT / QLoRA · PPO · garak · PyRIT · promptfoo · scikit-learn · SHAP / LIME · Opacus · FAISS · Scapy

Open to research collaboration in AI security and LLM red teaming.

*Offensive work is for research and for systems I am authorised to test.*
