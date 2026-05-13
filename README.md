# Arabic-FewShot-Autism-Dataset

Custom Arabic episodic dataset designed for few-shot learning and intent routing tasks in autism-support conversational AI systems.

## Overview

This repository contains a custom dataset created as part of a master's thesis research project. The dataset is organized into episodic tasks for meta-learning and few-shot classification experiments.

The dataset focuses on Arabic queries related to:
- autism support
- behavioral intervention
- educational guidance
- daily living skills
- adolescent autism care

Each episode follows a few-shot learning structure composed of:
- **Support set**
- **Query set**

using a **4-way 4-shot** configuration.

---

## Dataset Structure

Each episode is represented as:

```json
{
  "support": [
    {
      "query": "...",
      "route_id": 0
    }
  ],
  "query": [
    {
      "query": "...",
      "route_id": 1
    }
  ]
}
```

### Fields

| Field | Description |
|---|---|
| `query` | Arabic user query |
| `route_id` | Intent/category label |
| `support` | Few-shot support examples |
| `query` | Evaluation/test examples |

---

## Route Labels

The dataset contains multiple intent categories related to autism-support services and guidance.

Example categories include:
- Educational support
- Behavioral intervention
- Daily routines and independence
- Attention and engagement assessment

---

## Experimental Configuration

The dataset was divided into:
- Training episodes
- Testing episodes

All experiments were conducted using:
- **4-way classification**
- **4-shot learning**
- Episodic meta-learning setup

---

## Research Purpose

This dataset was created for research purposes in:
- Few-shot learning
- Meta-learning
- Arabic NLP
- Intent classification
- Conversational AI for autism support

---

## Citation

If you use this dataset in your research, please cite:

```bibtex
@dataset{arabic_autism_fsl_dataset,
  title={Arabic Few-Shot Autism Dataset},
  author={Your Name},
  year={2026}
}
```

---

## License

This dataset is released for academic and research purposes only.

---

## Keywords

`few-shot-learning` `meta-learning` `arabic-nlp` `autism` `intent-classification` `episodic-learning` `dataset`
