# Awesome Data Agent and Table Reasoning Paper

## Benchmark

### Data Agent Benchmark

| Benchmark Name | Corresp. Author     | Year | Source                                                                                  | TLDR |
|:--------------:|:-------------:|:----:|:---------------------------------------------------------------------------------------:|:-----|
| InfiAgent-DABench | Jingjing Xu | 2024 | [Link](https://arxiv.org/pdf/2401.05507) [Repo](https://github.com/InfiAgent/InfiAgent)| Input: NL data-analysis queries plus linked CSVs (executed in a constrained Python sandbox). Output: Closed-form answers in a fixed format (e.g., @answer_name[answer]). Metrics: Exact-match scoring on the canonicalized answers; aggregate accuracy over sub-tasks.
| CRAG | Xiao Yang | 2024 | [Link](https://arxiv.org/pdf/2406.04744) [Repo](https://github.com/facebookresearch/CRAG/)| Input: Factoid questions with access to provided corpora and mock retrieval/APIs. Output: Final textual answer (optionally with cited evidence). Metrics: Automatic correctness categories mapped to a score (correct/acceptable vs. missing/incorrect); report overall accuracy.
| FDABench | Gao Cong | 2025 | [Link](https://arxiv.org/pdf/2509.02473) [Repo](https://github.com/fdabench/FDAbench)| Input: Cross-source analytical queries spanning structured tables and unstructured sources. Output: Multiple-choice selections or a short analysis/report when required. Metrics: Exact-match for MC/checkbox tasks; text tasks by overlap metrics (e.g., ROUGE) plus tool-use success/recall; also reports efficiency (latency, model/tool calls, token/cost).
| DA-Bench | Yunjun Gao | 2025 | [Link](https://arxiv.org/pdf/2503.13269) [Repo](https://github.com/ZJU-LLMs/DAgent)| Input: Realistic analyst tasks against a live data stack/tools. Output: Final answers or produced charts/tables. Metrics: Per-task 0–5 rubric with penalties for extra user interaction, corrections, or hallucinations; summarize overall score and hallucination rate.

### Latest Benchmarks for Tabular Data (Since 2024)

| Benchmark Name | Task Type     | Year | Source                                                                                  | TLDR |
|:--------------:|:-------------:|:----:|:---------------------------------------------------------------------------------------:|:-----|
| MDBench        | Reasoning     | 2025 | [Link](https://github.com/jpeper/MDBench) | MDBench introduces a new multi-document reasoning benchmark synthetically generated through knowledge-guided prompting. |
| MMQA           | Reasoning     | 2025 | [Link](https://openreview.net/pdf?id=GGlpykXDCa)  [Repo](https://github.com/WuJian1995/MMQA/issues/2)| MMQA is a multi-table multi-hop question answering dataset with 3,312 tables across 138 domains, evaluating LLMs' capabilities in multi-table retrieval, Text-to-SQL, Table QA, and primary/foreign key selection.
| ToRR           | Reasoning     | 2025 | [Link](https://arxiv.org/pdf/2502.19412)  [Repo](https://github.com/IBM/unitxt/blob/main/prepare/benchmarks/torr.py)| ToRR is a benchmark assessing LLMs' table reasoning and robustness across 10 datasets with diverse table serializations and perturbations, revealing models' brittleness to format variations.
| MMTU           | Comprehensive | 2025 | [Link](https://arxiv.org/pdf/2506.05587)  [Repo](https://github.com/MMTU-Benchmark/MMTU)| MMTU is a massive multi-task table understanding and reasoning benchmark with over 30K questions across 25 real-world table tasks, designed to evaluate models' ability to understand, reason, and manipulate tables.
| RADAR          | Reasoning     | 2025 | [Link](https://kenqgu.com/assets/pdf/RADAR_ARXIV.pdf)  [Repo](https://huggingface.co/datasets/kenqgu/RADAR)| RADAR is a benchmark for evaluating language models' data-aware reasoning on imperfect tabular data with 5 common data artifact types like outlier value or inconsistent format, which ensures that direct calculation on the perturbed table will yield an incorrect answer, forcing the model to handle the artifacts to obtain the correct result.
| Spider2        | Text2SQL      | 2025 | [Link](https://arxiv.org/abs/2411.07763)  [Repo](https://github.com/xlang-ai/Spider2)|
| DataBench      | Reasoning     | 2024 | [Link](https://aclanthology.org/2024.lrec-main.1179.pdf)  [Repo](https://huggingface.co/datasets/cardiffnlp/databench)|
| TableBench     | Reasoning     | 2024 | [Link](https://arxiv.org/abs/2408.09174)  [Repo](https://github.com/TableBench/TableBench)|
| TQA-Bench      | Reasoning     | 2024 | [Link](https://arxiv.org/pdf/2411.19504)  [Repo](https://github.com/Relaxed-System-Lab/TQA-Bench)|
| SpreadsheetBench | Reasoning     | 2024 | [Link](https://arxiv.org/pdf/2406.14991)  [Repo](https://github.com/RUCKBReasoning/SpreadsheetBench/tree/main/data)|

### Selected Classical Reasoning Benchmarks for Tabular Data
| Benchmark Name | Task Type     | Year | Source                                                                                  | TLDR |
|:--------------:|:-------------:|:----:|:---------------------------------------------------------------------------------------:|:-----|
| FinQA          | Reasoning     | 2021 | [Link](https://arxiv.org/pdf/2109.00122)  [Repo](https://github.com/czyssrs/FinQA)|
| FeTaQA         | Reasoning     | 2021 | [Link](https://arxiv.org/pdf/2104.00369)  [Repo](https://github.com/Yale-LILY/FeTaQA)|
| HiTab          | Reasoning     | 2022 | [Link](https://aclanthology.org/2022.acl-long.78.pdf) [Repo](https://github.com/microsoft/HiTab)


## Conference Paper (including arxiv)
| Venue       | Paper                                                        | Corresp. Author |                           Links                             |
| :---------- | :----------------------------------------------------------- | :-------------: |:----------------------------------------------------------: | 
| SIGMOD'26   | ST-Raptor: LLM-Powered Semi-Structured Table Question Answering | Xuanhe Zhou |  [paper](https://arxiv.org/pdf/2508.18190)   |
| CIDR'25     | AOP: Automated and Interactive LLM Pipeline Orchestration for Answering Complex Queries | Guoliang Li |  [paper](https://www.vldb.org/cidrdb/papers/2025/p32-wang.pdf)   |
| VLDB'25     | Towards Automated Cross-domain Exploratory Data Analysis through Large Language Models  | Qi Liu | [paper](https://www.vldb.org/pvldb/vol18/p5086-zhu.pdf)   |
| VLDB'25     | AutoPrep: Natural Language Question-Aware Data Preparation with a Multi-Agent Framework | Qi Liu | [paper](https://www.vldb.org/pvldb/vol18/p5086-zhu.pdf)   |
| ICML'25     | Compositional Condition Question Answering in Tabular Understanding | Han-Jia Ye | [paper](https://www.vldb.org/pvldb/vol18/p5086-zhu.pdf?utm_source=chatgpt.com)   |
| ICML'25     | Are Large Language Models Ready for Multi-Turn Tabular Data Analysis? | Reynold Cheng | [paper](https://openreview.net/attachment?id=flKhxGTBj2&name=pdf) 
| NAACL'25    | H-STAR: LLM-driven Hybrid SQL-Text Adaptive Reasoning on Tables | Chandan K. Reddy | [paper](https://arxiv.org/pdf/2407.05952) 
| Neurips'25  | Table as a Modality for Large Language Models | Junbo Zhao| [paper](https://neurips.cc/virtual/2025/poster/116332)  
| Arxiv/2506  | MAPLE: Multi-Agent Adaptive Planning with Long-Term Memory for Table Reasoning | Thuy-Trang Vu |  [paper](https://arxiv.org/pdf/2503.13269)   |
| Arxiv/2503  | DAgent: A Relational Database-Driven Data Analysis Report Generation Agent | Yunjun Gao |  [paper](https://arxiv.org/pdf/2503.13269)   |
| Arxiv/2505  | TAIJI: MCP-based Multi-Modal Data Analytics on Data Lakes | Ju Fan |  [paper](https://arxiv.org/pdf/2505.11270)   |
| Arxiv/2508  | AgenticData: An Agentic Data Analytics System for Heterogeneous Data | Yuan Li |  [paper](https://arxiv.org/pdf/2508.50002)   |
| Arxiv'2501  | TableMaster: A Recipe to Advance Table Understanding with Language Models | Hanbing Liu |  [paper](https://arxiv.org/pdf/2501.19378)    |  |
| Arxiv'2505  | Weaver: Interweaving SQL and LLM for Table Reasoning | Vivek Gupta |  [paper](https://arxiv.org/pdf/2505.18961)    | 
| ICLR'24    | OpenTab: Advancing Large Language Models as Open-domain Table Reasoners | Jiani Zhang  |  [paper](https://arxiv.org/pdf/2402.14361)    | 
| ICLR'24    | CABINET: Content Relevance based Noise Reduction for Table Question Answering |  Balaji Krishnamurthy |  [paper](https://arxiv.org/pdf/2402.01155)    | 
| ICLR'24    | Chain-of-Table: Evolving Tables in the Reasoning Chain for Table Understanding | Tomas Pfister  |  [paper](https://arxiv.org/pdf/2401.04398)    |
| VLDB'24    | ReAcTable: Enhancing ReAct for Table Question Answering |  Jignesh M. Patel |  [paper](https://arxiv.org/pdf/2310.00815)    |
| VLDB'24    | AutoTQA: Towards Autonomous Tabular Question Answering through Multi-Agent Large Language Models | Qi Liu |  [paper](https://www.vldb.org/pvldb/vol17/p3920-zhu.pdf)    |
