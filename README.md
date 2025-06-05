# OriGene: A Self-Evolving Virtual Disease Biologist Automating Therapeutic Target Discovery

> **Important**: This is the Beta release of OriGene, the self-evolving multi-agent system that acts as a virtual disease biologist.
> We also introduce the TRQA Benchmark — a benchmark of 1,921 expert-level questions for evaluating biomedical AI agents.
> We will continue to release updated code incrementally over time.

<p align="center">
  | <a href="https://GENTEL-lab.io/OriGene">Homepage</a> |
  <a href="assets/OriGene.pdf">Paper</a> |
  <a href="https://github.com/GENTEL-lab/OriGene">Code</a> |
  <a href="https://huggingface.co/datasets/GENTEL-Lab/TRQA/">Hugging Face Benchmark</a> |
</p>



## 1. OriGene Overview
![Image](assets/OriGene_overview.jpg)
Therapeutic target discovery remains one of the most critical yet intuition-driven stages in drug development. We present **OriGene**, a self-evolving multi-agent system that functions as a virtual disease biologist to 
identify and prioritize therapeutic targets at scale. 

## 2. TRQA Benchmark Description
To evaluate performance, we constructed TRQA, a benchmark of 1,921 questions specific to therapeutic target identification tasks across multiple disease areas. 

![Image](assets/benchmark_construction.jpg)
![Image](assets/benchmark_description.jpg)

**Target Research-related Question Answering (TRQA) benchmark for evaluating biomedical knowledge and target identification skillsets.**
The TRQA is an evaluation dataset designed to systematically assess the comprehensive capacities of OriGene and other multi-agent 
frameworks in the field of therapeutic target discovery. TRQA focuses on key areas such as fundamental biology, disease 
biology, pharmacology, and clinical medicine, aiming to evaluate the ability to conduct effective planning, gather useful information, 
choose appropriate tools, reason to scientific conclusions, and critically self-evolve. It takes into account information from both 
extensive research literature and competitive landscape data related to drug R&D pipelines and clinical trials. 

TRQA consists of two sub-datasets: TRQA-lit, and TRQA-db.  TRQA-lit specifically focuses on research findings related to therapeutic targets, aiming to build a question-answering (QA) dataset 
from literature corpora that summarizes the latest research progress for well-recognized therapeutic targets.
It contains 172 multi-choice QAs (forming a core set for quick evaluation of models and humans) and 1,108 short-answer QAs, 
covering fundamental biology, disease biology, clinical medicine, and pharmacology.
TRQA-db is designed for  for systematically evaluating the effectiveness of information retrieval, integration, and reasoning among 
existing methods when addressing the competitive landscape investigation problem
It contains 641 short-answer QAs, which mainly focus on key competitive information of drug R\&D pipelines and clinical trials.

## 3. Evaluation Results
**Target Research-related Question Answering (TRQA) benchmark leader board**
| Method             | TRQA-lit Choice (Core Set) | TRQA-lit Short-Answer  | TRQA-db  |
|--------------------|----------------------------------|--------------------------------|------------------|
| Origene            | 0.601                            | 0.826                          | 0.721            |
| o3-mini            | 0.578                            | 0.720                          | 0.487            |
| Claude-3.7-Sonnet  | 0.558                            | 0.695                          | 0.504            |
| DeepSeek-R1        | 0.548                            | 0.714                          | 0.446            |
| DeepSeek-V3        | 0.541                            | 0.768                          | 0.466            |
| GPT-4o-search      | 0.531                            | 0.651                          | 0.493            |
| Gemini-2.5-pro     | 0.529                            | 0.678                          | 0.359            |
| GPT-4o             | 0.512                            | 0.696                          | 0.392            |
| TxAgent            | 0.190                            | 0.472                          | 0.426            |
| Human Group 3 (PhD + 3-5 year exp.)  | 0.523                            | ✗                          | ✗            |
| Human Group 2 (PhD + 1-3 year exp.)  | 0.378                            | ✗                          | ✗            |
| Human Group 1 (senior PhD candidates)  | 0.215                            | ✗                          | ✗            |

## The full source code is coming soon!
