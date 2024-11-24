# awesome-data-synthesis-for-code-llm
This is the repo for our survey paper [Mastering the Craft of Data Synthesis for CodeLLMs].
Repo for data synthesis and filtering techniques of Code LLMs, covering papers, datasets, benchmarks, and papers etc.

<p align='center'>
<img src='imgs/taxonomy.png' style='width: 100%; '>
</p>

## Table of Contents
1. [Open-source Synthetic datasets for Code LLMs](#1-datasets)

| Dataset    | Venue                            | Date              | Size                 | Language                                                                         | Source                                                                                                                                                                                                                                                                                       |
| ------- | -------------------------------- | ---------------------- | -------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Code Alpaca | Github                        | 2023                | 20K                 | Multi-lingual (Python, Java, C, ..., etc)                                                                             | "Code Alpaca: An Instruction-following LLaMA model for code generation" [[paper](https://github.com/sahil280114/codealpaca)], [[code](https://github.com/sahil280114/codealpaca)], [[data](https://huggingface.co/datasets/sahil2801/CodeAlpaca-20k)]
| WizardCoder | ICLR 2024                        | 2024                | 78K                 | Multi-lingual (Python, Java, C, ..., etc)                                                                             | "WizardCoder: Empowering Code Large Language Models with Evol-Instruct" [[paper](https://openreview.net/pdf?id=UnUwSIgK5W)], [[code](https://github.com/nlpxucan/WizardLM)], [[data](https://huggingface.co/datasets/WizardLMTeam/WizardLM_evol_instruct_70k)]
| Magicoder | ICML 2024                        | 2024                | 75K                 | Multi-lingual (Python, Java, C, ..., etc)                                                                             | "Magicoder: Source Code Is All You Need" [[paper](https://github.com/sahil280114/codealpaca)], [[code](https://github.com/ise-uiuc/magicoder)], [[data](https://huggingface.co/datasets/ise-uiuc/Magicoder-OSS-Instruct-75K)]
| CodeSeaXDataset |  NeurIPS 2024                       | 2024                | 20K                 | Multi-lingual (Python, Java, C, ..., etc)                                                                             | "WaveCoder: Widespread And Versatile Enhanced Code LLM" [[paper](https://arxiv.org/abs/2312.14187)], [[code](https://github.com/microsoft/WaveCoder)], [[data]()]
| PYX |  NeurIPS 2024                       | 2024                | 35K                 | Multi-lingual (Python, Java, C, ..., etc)                                                                             | "SemCoder: Training Code Language Models with Comprehensive Semantics Reasoning" [[paper](https://arxiv.org/pdf/2406.01006)], [[code](https://github.com/ARiSE-Lab/SemCoder)], [[data](https://huggingface.co/datasets/semcoder/PyX)]
| PYX-R |  NeurIPS 2024                       | 2024                | 19K                 | Multi-lingual (Python, Java, C, ..., etc)                                                                             | "SemCoder: Training Code Language Models with Comprehensive Semantics Reasoning" [[paper](https://arxiv.org/pdf/2406.01006)], [[code](https://github.com/ARiSE-Lab/SemCoder)], [[data](https://huggingface.co/datasets/semcoder/PyX-R)]
| AutoCoder-AIEV-Instruct |  Arxiv                       | 2024                | 169K                 | Multi-lingual (Python, Java, C, ..., etc)                                                                             | "AutoCoder: Enhancing Code Large Language Model with \textsc{AIEV-Instruct}" [[paper](https://arxiv.org/pdf/2405.14906)], [[code](https://github.com/bin123apple/AutoCoder)], [[data]()]
| MultiPL-T |  ACM Program. Lang                       | 2024                | 215K                 | Low resource language (Lua, Racket, Ocamal, Julia/r)                                                                             | "Knowledge Transfer from High-Resource to Low-Resource Programming Languages for Code LLMs" [[paper](https://arxiv.org/pdf/2308.09895)], [[code](https://github.com/nuprl/MultiPL-T)], [[data](https://huggingface.co/datasets/nuprl/MultiPL-T)]
| CodeUltraFeedback |  Arxiv                       | 2024                | 10K                 | Multi-lingual (Python, Java, C, ..., etc)                                                                             | "CodeUltraFeedback: An LLM-as-a-Judge Dataset for Aligning Large Language Models to Coding Preferences" [[paper](https://arxiv.org/abs/2403.09032)], [[code](https://github.com/martin-wey/CodeUltraFeedback)], [[data](https://huggingface.co/datasets/coseal/CodeUltraFeedback)]
| CRUXEval |  Arxiv                       | 2024                | 800                 | Python                                                                             | "CRUXEval: A Benchmark for Code Reasoning, Understanding and Execution" [[paper](https://arxiv.org/abs/2401.03065)], [[code](https://github.com/facebookresearch/cruxeval)], [[data](https://huggingface.co/datasets/cruxeval-org/cruxeval)]
| AmbiQT |  EMNLP 2023                       | 2023                | 3000                 | SQL                                                                             | "Benchmarking and Improving Text-to-SQL Generation Under Ambiguity" [[paper](https://aclanthology.org/2023.emnlp-main.436.pdf)], [[code](https://github.com/testzer0/AmbiQT)], [[data](https://github.com/testzer0/AmbiQT/tree/master/benchmark)]
| Dr.Spider |  ICLR 2023                       | 2023                | 15K                 | SQL                                                                             | "Dr. Spider: A Diagnostic Evaluation Benchmark towards Text-to-SQL Robustness" [[paper](https://arxiv.org/abs/2301.08881)], [[code](https://github.com/awslabs/diagnostic-robustness-text-to-sql)], [[data](https://github.com/awslabs/diagnostic-robustness-text-to-sql/blob/main/data.tar.gz)]
| ScienceBenchmark |  Arxiv                       | 2023                | 4K                 | SQL                                                                             | "ScienceBenchmark: A Complex Real-World Benchmark for Evaluating Natural Language to SQL Systems" [[paper](https://arxiv.org/abs/2306.04743)], [[code](https://github.com/yizhang-unifr/nl-ql-data-augmentation)], [[data](https://github.com/ckosten/sciencebenchmark_dataset)]
|CodePLAN |  LREC 2024                       | 2024                | 11K                 | Python                                                                             | "Enhancing Code Generation Performance of Smaller Models by Distilling the Reasoning Ability of LLMs" [[paper](https://aclanthology.org/2024.lrec-main.521.pdf)], [[code](https://github.com/sssszh/CodePLAN)], [[data](https://github.com/sssszh/CodePLAN)]
| OpenCodeInterpreter |  ACL 2024 Findings                      | 2024                | 68K                 | Python                                                                             | "OpenCodeInterpreter: Integrating Code Generation with Execution and Refinement" [[paper](https://aclanthology.org/2024.findings-acl.762.pdf)], [[code](https://github.com/OpenCodeInterpreter/OpenCodeInterpreter)], [[data](https://huggingface.co/datasets/m-a-p/Code-Feedback)]
| DebugBench |  ACL 2024 Findings                      | 2024                | 4K                 | Python, Java, C++                                                                             | "DebugBench: Evaluating Debugging Capability of Large Language Models" [[paper](https://aclanthology.org/2024.findings-acl.247.pdf)], [[code](https://github.com/thunlp/DebugBench)], [[data](https://huggingface.co/datasets/Rtian/DebugBench)]
| DistiLRR |  Arxiv                       | 2024                | 7K                 | Python, Java, Javascript, Perl, Golang, Swift                                                                             | "DistiLRR: Transferring Code Repair for Low-Resource Programming Languages" [[paper](https://arxiv.org/pdf/2406.14867)], [[code](https://github.com/KyleWong288/Distill_LRPL)], [[data](https://github.com/KyleWong288/Distill_LRPL)]
| PIE |  ICLR 2024                       | 2024                | 1.5K                 | Python                                                                             | "Learning Performance-Improving Code Edits" [[paper](https://openreview.net/pdf?id=ix7rLVHXyY)], [[code](https://github.com/LearningOpt/pie)], [[data](https://github.com/LearningOpt/pie?tab=readme-ov-file#dataset)]
| CodeExp |  EMNLP 2022 Findings                       | 2022                | 13K                 | Python                                                                             | "SemCoder: Training Code Language Models with Comprehensive Semantics Reasoning" [[paper](https://aclanthology.org/2022.findings-emnlp.174.pdf)], [[code](https://github.com/subercui/CodeExp)], [[data](https://github.com/subercui/CodeExp/blob/main/dataset/CodeExp(annotated)13k.json)]
| Jam-CGPT |  Automated Software Engineering 2024                       | 2024                | 2.15M                 | Java                                                                             | "Distilled GPT for Source Code Summarization" [[paper](https://arxiv.org/pdf/2308.14731)], [[code](https://github.com/apcl-research/Jam-CGPT)], [[data](https://huggingface.co/datasets/apcl/Jam-CGPT/tree/main)]



2. [Benchmarking for Code LLMs](#2-benchmarking)

- [NeurIPS 2021] **CodeXGLUE**: "CodeXGLUE: A Machine Learning Benchmark Dataset for Code Understanding and Generation", [[paper](https://arxiv.org/abs/2102.04664)] [[repo](https://github.com/microsoft/CodeXGLUE)]

- [Arxiv 2021] **HumanEval**: "Evaluating Large Language Models Trained on Code", [[paper](https://arxiv.org/abs/2107.03374)] [[repo](https://github.com/openai/human-eval)]

- [Arxiv 2021] **MBPP**: "Program Synthesis with Large Language Models", [[paper](https://arxiv.org/abs/2108.07732)] [[repo](https://github.com/google-research/google-research/tree/master/mbpp)]

- [Arxiv 2022] **DS-1000**: "DS-1000: A Natural and Reliable Benchmark for Data Science Code Generation", [[paper](https://arxiv.org/abs/2211.11501)] [[repo](https://github.com/xlang-ai/DS-1000)]

- [Arxiv 2023] **HumanEval+**: "Is Your Code Generated by ChatGPT Really Correct? Rigorous Evaluation of Large Language Models for Code Generation", [[paper](https://arxiv.org/abs/2305.01210)] [[repo](https://github.com/evalplus/evalplus)]

- [Arxiv 2023] **HumanEvalPack**, "OctoPack: Instruction Tuning Code Large Language Models", [[paper](https://arxiv.org/abs/2308.07124)] [[repo](https://huggingface.co/datasets/bigcode/humanevalpack)]

- [Arxiv 2024] **BigCodeBench**: "BigCodeBench: Benchmarking Code Generation with Diverse Function Calls and Complex Instructions", [[paper](https://arxiv.org/abs/2406.15877)] [[repo](https://github.com/bigcode-project/bigcodebench)]

- [Arxiv 2024] **LiveCodeBench**: "LiveCodeBench: Holistic and Contamination Free Evaluation of Large Language Models for Code", [[paper](https://arxiv.org/abs/2403.07974)] [[repo](https://github.com/LiveCodeBench/LiveCodeBench)]

- [IEEE Trans. Software Engineering 2022] **MultiPL-E**: "MultiPL-E: A Scalable and Extensible Approach to Benchmarking Neural Code Generation", [[paper](https://arxiv.org/abs/2208.08227)] [[repo](https://github.com/nuprl/MultiPL-E)]

- [Arxiv 2024] **McEval**: "McEval: Massively Multilingual Code Evaluation", [[paper](https://arxiv.org/abs/2406.07436)] [[repo](https://github.com/MCEVAL/McEval)] 

- [ICML 2024] **CRUXEval**: "CRUXEval: A Benchmark for Code Reasoning, Understanding and Execution", [[paper](https://arxiv.org/abs/2401.03065)] [[repo](https://github.com/facebookresearch/cruxeval)] 

- [2024] **Aider**: "Aider is AI pair programming in your terminal", [[repo](https://github.com/Aider-AI/aider)]

- [Arxiv 2024] **Long Code Arena**: "Long Code Arena: a Set of Benchmarks for Long-Context Code Models", [[paper](https://arxiv.org/abs/2406.11612)] [[repo](https://github.com/JetBrains-Research/lca-baselines)]

- [2024] **DebugEval**: Enhancing the Code Debugging Ability of LLMs via Communicative Agent Based Data Refinement [[paper](https://arxiv.org/abs/2408.05006)] [[repo](https://github.com/NEUIR/DebugEval)]

- [EMNLP 2018] **Spider**: "Spider: A Large-Scale Human-Labeled Dataset for Complex and Cross-Domain Semantic Parsing and Text-to-SQL Task", [[paper](https://arxiv.org/abs/1809.08887)] [[repo](https://yale-lily.github.io/spider)]

- [Arxiv 2023] **BIRD**: "Can LLM Already Serve as A Database Interface? A BIg Bench for Large-Scale Database Grounded Text-to-SQLs", [[paper](https://arxiv.org/abs/2305.03111)] [[repo](https://bird-bench.github.io/)]

- 🔥[Arxiv 2024] **Spider 2.0**: "Spider 2.0: Evaluating Language Models on Real-World Enterprise Text-to-SQL Workflows", [[paper](https://arxiv.org/abs/2411.07763)] [[repo](https://github.com/xlang-ai/Spider2)]



3. [Recommended Open-source LLMs](#3-recommended-llms)

- **Llama-3.1-405B**: <img src="https://huggingface.co/front/assets/huggingface_logo.svg" alt="Hugging Face" width="20"> https://huggingface.co/meta-llama/Llama-3.1-405B

- **Llama-3.2-90B**: <img src="https://huggingface.co/front/assets/huggingface_logo.svg" alt="Hugging Face" width="20"> https://huggingface.co/meta-llama/Llama-3.2-90B-Vision-Instruct

- **Qwen2.5-72B-Instruct-GGUF**: <img src="https://huggingface.co/front/assets/huggingface_logo.svg" alt="Hugging Face" width="20"> https://huggingface.co/Qwen/Qwen2.5-72B-Instruct-GGUF

- **DeepSeek-Coder-V2-Instruct**: <img src="https://huggingface.co/front/assets/huggingface_logo.svg" alt="Hugging Face" width="20"> https://huggingface.co/deepseek-ai/DeepSeek-Coder-V2-Instruct

- **Qwen2.5-Coder-32B-Instruct**: <img src="https://huggingface.co/front/assets/huggingface_logo.svg" alt="Hugging Face" width="20"> https://huggingface.co/Qwen/Qwen2.5-Coder-32B-Instruct

- **Starcoder2-15b**: <img src="https://huggingface.co/front/assets/huggingface_logo.svg" alt="Hugging Face" width="20"> https://huggingface.co/bigcode/starcoder2-15b



4. [Papers](#4-papers)

  - 4.1 [Data Synthesis](#41-data-synthesis)

  - 4.2 [Data Filtering](#42-coding-filtering)

