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
| Code Alpaca | Github                        | 2023                | 20K                 | Multi-lingual (Python/Java/C/...)                                                                             | "Code Alpaca: An Instruction-following LLaMA model for code generation" [[paper](https://github.com/sahil280114/codealpaca)], [[code](https://github.com/sahil280114/codealpaca)], [[data](https://huggingface.co/datasets/sahil2801/CodeAlpaca-20k)]
| WizardCoder | ICLR 2024                        | 2024                | 78K                 | Multi-lingual (Python/Java/C/...)                                                                             | "WizardCoder: Empowering Code Large Language Models with Evol-Instruct" [[paper](https://openreview.net/pdf?id=UnUwSIgK5W)], [[code](https://github.com/nlpxucan/WizardLM)], [[data](https://huggingface.co/datasets/WizardLMTeam/WizardLM_evol_instruct_70k)]
| Magicoder | ICML 2024                        | 2024                | 75K                 | Multi-lingual (Python/Java/C/...)                                                                             | "Magicoder: Source Code Is All You Need" [[paper](https://github.com/sahil280114/codealpaca)], [[code](https://github.com/ise-uiuc/magicoder)], [[data](https://huggingface.co/datasets/ise-uiuc/Magicoder-OSS-Instruct-75K)]
| CodeSeaXDataset |  NeurIPS 2024                       | 2024                | 20K                 | Multi-lingual (Python/Java/C/...)                                                                             | "WaveCoder: Widespread And Versatile Enhanced Code LLM" [[paper](https://arxiv.org/abs/2312.14187)], [[code](https://github.com/microsoft/WaveCoder)], [[data]()]
| PYX |  NeurIPS 2024                       | 2024                | 35K                 | Multi-lingual (Python/Java/C/...)                                                                             | "SemCoder: Training Code Language Models with Comprehensive Semantics Reasoning" [[paper](https://arxiv.org/pdf/2406.01006)], [[code](https://github.com/ARiSE-Lab/SemCoder)], [[data](https://huggingface.co/datasets/semcoder/PyX)]
| PYX-R |  NeurIPS 2024                       | 2024                | 19K                 | Multi-lingual (Python/Java/C/...)                                                                             | "SemCoder: Training Code Language Models with Comprehensive Semantics Reasoning" [[paper](https://arxiv.org/pdf/2406.01006)], [[code](https://github.com/ARiSE-Lab/SemCoder)], [[data](https://huggingface.co/datasets/semcoder/PyX-R)]
| AutoCoder-AIEV-Instruct |  Arxiv                       | 2024                | 169K                 | Multi-lingual (Python/Java/C/...)                                                                             | "AutoCoder: Enhancing Code Large Language Model with \textsc{AIEV-Instruct}" [[paper](https://arxiv.org/pdf/2405.14906)], [[code](https://github.com/bin123apple/AutoCoder)], [[data]()]
| MultiPL-T |  ACM Program. Lang                       | 2024                | 215K                 | Multi-lingual (Lua/racket/ocamal/julia/r)                                                                             | "Knowledge Transfer from High-Resource to Low-Resource Programming Languages for Code LLMs" [[paper](https://arxiv.org/pdf/2308.09895)], [[code](https://github.com/nuprl/MultiPL-T)], [[data](https://huggingface.co/datasets/nuprl/MultiPL-T)]

| CodeSeaXDataset |  NeurIPS 2024                       | 2024                | 19K                 | Multi-lingual (Python/Java/C/...)                                                                             | "SemCoder: Training Code Language Models with Comprehensive Semantics Reasoning" [[paper]()], [[code]()], [[data]()]

2. [Benchmarking for Code LLMs](#2-benchmarking)

3. [Recommended LLMs](#3-recommended-llms)

4. [Papers](#4-papers)

  4.1 [Data Synthesis](#41-data-synthesis)

  4.2 [Data Filtering](#42-coding-filtering)

