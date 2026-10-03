# M Talha

**AI security engineer** · LLM security · evaluation of security machine learning

I build and stress-test machine-learning systems for cybersecurity. One question runs through all of my work: **do the results still hold when conditions change?** That means a new network, an attacker who adapts, a stricter privacy budget, or an analyst who has to trust an explanation.

## Research projects

### Security with and of language models

| Project | What it asks | Headline result |
|---|---|---|
| [**MCASM**](https://github.com/xorai-sec/mcasm-multicloud-attack-surface-slm) | Can a 3B-parameter model fine-tuned with QLoRA triage multi-cloud security findings like an expert? | Kendall τ-b 0.745 vs 0.066 untrained. It matches a hand-built rule system on expert agreement (0.848 vs 0.800, not significant) and adds explanations. |
| [**RAG-Sentinel**](https://github.com/xorai-sec/rag-sentinel) | Can retrieved text be screened for hidden instructions before it reaches the LLM? | Attack success 35.4% → 1.0% in simulation. The evaluation also uncovers a dataset shortcut and treats the in-domain scores as upper bounds. |

### Evaluating machine learning for defence

| Project | What it asks | Headline result |
|---|---|---|
| [**Federated DP-IDS**](https://github.com/xorai-sec/federated-dp-ids) | What do federation and differential privacy cost an intrusion detector? | Federation is free (F1 0.9947 vs 0.9944). ε = 1 costs 1.3 points, and a memorisation audit falls to chance. |
| [**NIDS Benchmark Reality Check**](https://github.com/xorai-sec/nids-benchmark-reality-check) | How much of a 99.99% benchmark score survives a change of network? | In-dataset PR-AUC 0.99996 falls to 0.07–0.24 across datasets. |
| [**NIDS PCAP Deployment Gap**](https://github.com/xorai-sec/nids-pcap-deployment-gap) | Does benchmark accuracy predict behaviour on independently extracted traffic? | 99.9% on the benchmark; a Random Forest flagged none of 3,978 malicious flows from raw PCAP. |
| [**Explainable Malware Detection**](https://github.com/xorai-sec/explainable-malware-detection) | Can we measure whether SHAP/LIME explanations deserve trust? | Accurate models, faithful explanations (0.92), but unstable (0.44) and inconsistent across methods (0.15). |

## How I work

- **Leak-free by design:** group-aware splits, preprocessing fitted on training data only, automated leakage checks.
- **Report the uncomfortable result:** each repository has a section on what the evidence does *not* show.
- **Reproducible:** pinned sources, saved outputs, notebooks that run end to end on Colab.

## Toolbox

Python · PyTorch · Hugging Face Transformers / PEFT (QLoRA) · scikit-learn · XGBoost / LightGBM · Opacus (DP-SGD) · SHAP / LIME · Scapy · Streamlit

## Contact

m.talha@cytomate.net
