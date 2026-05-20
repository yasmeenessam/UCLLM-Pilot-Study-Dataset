# UCLLM Pilot Study Dataset

This repository contains the anonymized datasets associated with the paper:

**Beyond Benchmarks: A User-Centric Framework for Evaluating Large Language Models**

The released materials support transparency and reproducibility for the pilot study evaluating the *Trust & Transparency* dimension of UCLLM through epistemic stance manipulation.

---

# Repository Contents

```text
ucllm/
├── participant_ratings.csv
├── chat_logs_cleaned.csv
└── README.md
```

---

# Files

## `participant_ratings.csv`

This file contains de-identified participant ratings collected after each interaction condition.

### Included Measures

Participants rated the following items on a 7-point Likert scale:

1. *“The assistant seemed confident in its recommendations.”*
2. *“The assistant’s recommendations felt reliable and trustworthy.”*
3. *“The assistant provided advice I would feel comfortable following.”*
4. *“I enjoyed interacting with this assistant.”*

Response scale:

- 1 = Strongly disagree
- 7 = Strongly agree

### Main Columns

| Column | Description |
|---|---|
| participant_id | anonymized participant identifier |
| model | evaluated LLM |
| stance_condition | high-certainty or low-certainty condition |
| perceived_certainty | certainty rating |
| trust_reliability | trustworthiness rating |
| actionability | usefulness/actionability rating |
| overall_enjoyment | enjoyment rating |

---

## `chat_logs_cleaned.csv`

This file contains anonymized participant–LLM interaction logs.

Each row represents a single conversational message.

### Main Columns

| Column | Description |
|---|---|
| interaction_id | unique interaction/session identifier |
| participant_id | anonymized participant identifier |
| model | evaluated LLM |
| stance_condition | high-certainty or low-certainty condition |
| context | interaction scenario |
| exchange_number | conversational exchange index |
| message_order | message sequence order |
| speaker | participant or assistant |
| message | conversational content |

### Privacy

To preserve participant privacy:

- participant identifiers were anonymized
- timestamps were removed
- personally identifying content was excluded where necessary

---

# Study Overview

The study examined how epistemic stance (high-certainty vs. low-certainty language) influences user perceptions of LLM behavior.

Participants interacted with four LLMs across eight within-subject conditions.

The pilot investigates the *Trust & Transparency* dimension of UCLLM.

---
# Citation

If you use this dataset, please cite:

```bibtex
@inproceedings{10.1145/3816046.3816227,
author = {Yasmeen Abdrabou, Yomna Abdelrahman, Efe Bozkir, Youssef Mazen, Florian Alt, and Enkelejda Kasneci},
title = {Beyond Benchmarks: A User-Centric Framework for Evaluating Large Language Models},
year = {2026},
publisher = {Association for Computing Machinery},
address = {New York, NY, USA},
url = {https://doi.org/110.1145/3816046.3816227},
doi = {10.1145/3816046.3816227},
series = {CUI '26}
}
```

---


# License

Released for academic and research use.
