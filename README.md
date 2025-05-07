# 🛡️ Guardling

*A lightweight linguistic guardrail for safer text generation.*

---

## 🚀 Overview

**Guardling** is a fine-tuned BERT-based model trained on the [ToxiGen](https://arxiv.org/abs/2203.09509) dataset to detect and score toxicity in generated text.
It is designed to act as a **small, efficient guardrail** — helping AI applications filter, evaluate, or discourage toxic outputs in real-time.

This repository covers:

*  Fine-tuning on ToxiGen
* Evaluation and scoring scripts
* Exported model ready to plug into larger AI pipelines (e.g., RLHF setups, chatbots)

---

## Use Cases

* **Safety scoring** for LLM outputs
* Toxicity filtering in chatbots and multi-agent systems
* Research on responsible AI and alignment
* Input guardrails for fine-tuning / RLHF pipelines

---

## Project Structure

```
guardling/
│
├── data/
│   └── toxigen_dataset/
│
├── scripts/
│   ├── train.py
│   ├── evaluate.py
│   ├── predict.py  # Easy API to score text
│   └── utils.py
│
├── models/
│   └── fine_tuned_guardling/
│
├── notebooks/
│   └── training_exploration.ipynb
│
├── requirements.txt
└── README.md
```

---


## Why *Guardling*?

* **Small & efficient**: Built to be lightweight but powerful
* **Plug-and-play**: Easily integrate as a scoring component in any AI pipeline
* **Research-aligned**: Fine-tuned on SOTA ToxiGen dataset
* **Linguistically aware**: Tailored for nuanced toxicity detection


## Future Plans

* [ ] Upload fine-tuned model to Hugging Face Hub
* [ ] Add multi-lingual support
* [ ] Integrate calibration methods for better thresholding

---

## Related Projects

* [ToxiGen Dataset](https://github.com/microsoft/ToxiGen)
* Phase 2: RLHF Debate Safety Study coming soon! [Discovering Language Model Behaviors with Model-Written Evaluations](https://aclanthology.org/2023.findings-acl.847/) (Perez et al., Findings 2023)

---

## 🛡️ License

MIT License. Feel free to use and modify with attribution.

---

## Acknowledgements

* ToxiGen authors and dataset creators
* Inspiration from HateBERT and CivilityClassifier projects


