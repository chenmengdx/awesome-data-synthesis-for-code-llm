# awesome-data-synthesis-for-code-llm
This is the repo for our survey paper [Mastering the Craft of Data Synthesis for CodeLLMs].
Repo for data synthesis and filtering techniques of Code LLMs, covering papers, datasets, benchmarks, and papers etc.

<p align='center'>
<img src='imgs/taxonomy.png' style='width: 100%; '>
</p>

## Table of Contents
1. [Synthetic datasets for Code LLMs](#1-datasets)

| Dataset    | Venue                            | Date              | Size                 | Language                                                                         | Source                                                                                                                                                                                                                                                                                       |
| ------- | -------------------------------- | ---------------------- | -------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Code Alpaca | Github                        | 2023                | 20K                 | Multi-lingual (Python, Java, C, ...)                                                                             | "Code Alpaca: An Instruction-following LLaMA model for code generation" [[paper](https://github.com/sahil280114/codealpaca)], [[code](https://github.com/sahil280114/codealpaca)], [[data](https://huggingface.co/datasets/sahil2801/CodeAlpaca-20k)]
| WizardCoder | ICLR 2024                        | 2024                | 78K                 | Multi-lingual (Python/Java/C/...)                                                                             | "WizardCoder: Empowering Code Large Language Models with Evol-Instruct" [[paper](https://openreview.net/pdf?id=UnUwSIgK5W)], [[code](https://github.com/nlpxucan/WizardLM)], [[data](https://huggingface.co/datasets/WizardLMTeam/WizardLM_evol_instruct_70k)]
| Magicoder | ICML 2024                        | 2024                | 75K                 | Multi-lingual (Python/Java/C/...)                                                                             | "Magicoder: Source Code Is All You Need" [[paper](https://github.com/sahil280114/codealpaca)], [[code](https://github.com/ise-uiuc/magicoder)], [[data](https://huggingface.co/datasets/ise-uiuc/Magicoder-OSS-Instruct-75K)]
| CodeSeaXDataset |  NeurIPS 2024                       | 2024                | 20K                 | Multi-lingual (Python/Java/C/...)                                                                             | "WaveCoder: Widespread And Versatile Enhanced Code LLM" [[paper](https://arxiv.org/abs/2312.14187)], [[code](https://github.com/microsoft/WaveCoder)], [[data]()]
| PYX |  NeurIPS 2024                       | 2024                | 35K                 | Multi-lingual (Python/Java/C/...)                                                                             | "SemCoder: Training Code Language Models with Comprehensive Semantics Reasoning" [[paper](https://arxiv.org/pdf/2406.01006)], [[code](https://github.com/ARiSE-Lab/SemCoder)], [[data](https://huggingface.co/datasets/semcoder/PyX)]
| PYX-R |  NeurIPS 2024                       | 2024                | 19K                 | Multi-lingual (Python/Java/C/...)                                                                             | "SemCoder: Training Code Language Models with Comprehensive Semantics Reasoning" [[paper](https://arxiv.org/pdf/2406.01006)], [[code](https://github.com/ARiSE-Lab/SemCoder)], [[data](https://huggingface.co/datasets/semcoder/PyX-R)]
| AutoCoder-AIEV-Instruct |  Arxiv                       | 2024                | 169K                 | Multi-lingual (Python/Java/C/...)                                                                             | "AutoCoder: Enhancing Code Large Language Model with \textsc{AIEV-Instruct}" [[paper](https://arxiv.org/pdf/2405.14906)], [[code](https://github.com/bin123apple/AutoCoder)], [[data]()]
| MultiPL-T |  ACM Program. Lang                       | 2024                | 215K                 | Low resource language (Lua/racket/ocamal/julia/r)                                                                             | "Knowledge Transfer from High-Resource to Low-Resource Programming Languages for Code LLMs" [[paper](https://arxiv.org/pdf/2308.09895)], [[code](https://github.com/nuprl/MultiPL-T)], [[data](https://huggingface.co/datasets/nuprl/MultiPL-T)]
| CodeUltraFeedback |  Arxiv                       | 2024                | 10K                 | Multi-lingual (Python/Java/C/...                                                                             | "CodeUltraFeedback: An LLM-as-a-Judge Dataset for Aligning Large Language Models to Coding Preferences" [[paper](https://arxiv.org/abs/2403.09032)], [[code](https://github.com/martin-wey/CodeUltraFeedback)], [[data](https://huggingface.co/datasets/coseal/CodeUltraFeedback)]
| CRUXEval |  Arxiv                       | 2024                | 800                 | Python                                                                             | "CRUXEval: A Benchmark for Code Reasoning, Understanding and Execution" [[paper](https://arxiv.org/abs/2401.03065)], [[code](https://github.com/facebookresearch/cruxeval)], [[data](https://huggingface.co/datasets/cruxeval-org/cruxeval)]
| AmbiQT |  EMNLP 2023                       | 2023                | 3000                 | SQL                                                                             | "Benchmarking and Improving Text-to-SQL Generation Under Ambiguity" [[paper](https://aclanthology.org/2023.emnlp-main.436.pdf)], [[code](https://github.com/testzer0/AmbiQT)], [[data](https://github.com/testzer0/AmbiQT/tree/master/benchmark)]
| Dr.Spider |  ICLR 2023                       | 2023                | 15K                 | SQL                                                                             | "Dr. Spider: A Diagnostic Evaluation Benchmark towards Text-to-SQL Robustness" [[paper](https://arxiv.org/abs/2301.08881)], [[code](https://github.com/awslabs/diagnostic-robustness-text-to-sql)], [[data](https://github.com/awslabs/diagnostic-robustness-text-to-sql/blob/main/data.tar.gz)]
| ScienceBenchmark |  Arxiv                       | 2023                | 4K                 | SQL                                                                             | "ScienceBenchmark: A Complex Real-World Benchmark for Evaluating Natural Language to SQL Systems" [[paper](https://arxiv.org/abs/2306.04743)], [[code](https://github.com/yizhang-unifr/nl-ql-data-augmentation)], [[data](https://github.com/ckosten/sciencebenchmark_dataset)]
|CodePLAN |  LREC 2024                       | 2024                | 11K                 | Python                                                                             | "Enhancing Code Generation Performance of Smaller Models by Distilling the Reasoning Ability of LLMs" [[paper](https://aclanthology.org/2024.lrec-main.521.pdf)], [[code](https://github.com/sssszh/CodePLAN)], [[data](https://github.com/sssszh/CodePLAN)]
| OpenCodeInterpreter |  ACL 2024 Findings                      | 2024                | 68K                 | Python                                                                             | "OpenCodeInterpreter: Integrating Code Generation with Execution and Refinement" [[paper](https://aclanthology.org/2024.findings-acl.762.pdf)], [[code](https://github.com/OpenCodeInterpreter/OpenCodeInterpreter)], [[data](https://huggingface.co/datasets/m-a-p/Code-Feedback)]
| DebugBench |  ACL 2024 Findings                      | 2024                | 4K                 | Python/Java/C++                                                                             | "DebugBench: Evaluating Debugging Capability of Large Language Models" [[paper](https://aclanthology.org/2024.findings-acl.247.pdf)], [[code](https://github.com/thunlp/DebugBench)], [[data](https://huggingface.co/datasets/Rtian/DebugBench)]
| DistiLRR |  Arxiv                       | 2024                | 7K                 | Python/Java/Javascript/Perl/Golang/Swift                                                                             | "DistiLRR: Transferring Code Repair for Low-Resource Programming Languages" [[paper](https://arxiv.org/pdf/2406.14867)], [[code](https://github.com/KyleWong288/Distill_LRPL)], [[data](https://github.com/KyleWong288/Distill_LRPL)]
| PIE |  ICLR 2024                       | 2024                | 1.5K                 | Python                                                                             | "Learning Performance-Improving Code Edits" [[paper](https://openreview.net/pdf?id=ix7rLVHXyY)], [[code](https://github.com/LearningOpt/pie)], [[data](https://github.com/LearningOpt/pie?tab=readme-ov-file#dataset)]
| CodeExp |  EMNLP 2022 Findings                       | 2022                | 13K                 | Python                                                                             | "SemCoder: Training Code Language Models with Comprehensive Semantics Reasoning" [[paper](https://aclanthology.org/2022.findings-emnlp.174.pdf)], [[code](https://github.com/subercui/CodeExp)], [[data](https://github.com/subercui/CodeExp/blob/main/dataset/CodeExp(annotated)13k.json)]
| Jam-CGPT |  Automated Software Engineering 2024                       | 2024                | 2.15M                 | Java                                                                             | "Distilled GPT for Source Code Summarization" [[paper](https://arxiv.org/pdf/2308.14731)], [[code](https://github.com/apcl-research/Jam-CGPT)], [[data](https://huggingface.co/datasets/apcl/Jam-CGPT/tree/main)]

2. [Benchmarking for Code LLMs](#2-benchmarking)

3. [Recommended LLMs](#3-recommended-llms)

4. [Papers](#4-papers)

  4.1 [Data Synthesis](#41-data-synthesis)

  4.2 [Data Filtering](#42-coding-filtering)

