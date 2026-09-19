# Human vs. AI-Rewritten Bengali Text Detection Dataset

A benchmark dataset for detecting **AI-rewritten Bengali text from authentic human-written Bengali text**.

This dataset contains paired Bengali texts consisting of original human-written passages and their corresponding AI-rewritten versions. It is designed to support research in **AI-rewritten text detection, Bengali Natural Language Processing (NLP), stylometric analysis, authorship attribution, paraphrase identification, and related tasks**.

---

## Dataset Overview

The dataset contains **4,000 Bengali text samples**, organized into **2,000 human–AI text pairs**.

| Statistic | Value |
|---|---:|
| Total Samples | 4,000 |
| Human-written Texts | 2,000 |
| AI-Rewritten Texts | 2,000 |
| Unique Pair_IDs | 2,000 |
| Human–AI Pairs | 2,000 |

Each human-written text is paired with its corresponding AI-rewritten version through a unique `Pair_ID`.

The AI-rewritten texts were generated using multiple large language models, including **ChatGPT, Claude, Gemini, and DeepSeek**, using a standardized rewriting procedure designed to preserve the original semantic meaning as much as possible.

---

## Data Sources

The human-written texts were collected from authentic Bengali sources representing multiple content domains, including:

- **National Curriculum and Textbook Board (NCTB)** textbooks
- **Bengali literary works available through Wikisource**
- **Bengali news articles published before 2020**

The dataset covers multiple content domains, including:

- Education
- Bengali Literature
- News

These sources provide naturally written Bengali texts from different domains and writing styles.

---

## Dataset Structure

The main dataset contains the following fields:

| Column | Description |
|---|---|
| `ID` | Unique identifier assigned to each individual text instance |
| `Pair_ID` | Identifier linking a human-written text with its corresponding AI-rewritten text |
| `Text` | Bengali text content |
| `Source` | Original source of the human text or the AI rewriting model |
| `Category` | Content domain, such as Education, Literature, or News |
| `Word_Count` | Number of words in the text |
| `Label` | Class label: `Human` or `AI-Rewritten` |

---

## Human–AI Pair Structure

Each original human-written text and its corresponding AI-rewritten text share the same `Pair_ID`.

For example:

```text
Pair_ID: bn_001

Human:
[Original Bengali text]

AI-Rewritten:
[Corresponding AI-rewritten Bengali text]
