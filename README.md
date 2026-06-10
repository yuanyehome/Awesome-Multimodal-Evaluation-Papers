# 🔬 Awesome Multimodal Foundation Model Evaluations

<div align="center">

![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/)

</div>

<p align="center">
  <img src="figs/main.jpg" width="90%" alt="Multimodal Foundation Model Evaluations Overview">
</p>

## 🌟 Overview

This repository tracks research papers on **Multimodal Foundation Model Evaluations** and serves as the companion paper list for the survey **"A Comprehensive Survey of Evaluating Multimodal Foundation Models: Hierarchical Perspective and Extensive Applications."**

The survey organizes the evaluation landscape through a three-level hierarchy: **fundamental competencies**, **higher-order intelligence**, and **real-world applications**. This README is synchronized with the TKDE manuscript version that uses a May 2025 corpus snapshot for visual analysis and a June 2026 snapshot for the representative benchmark comparison.

The maintained corpus is built from academic indexes, venue proceedings, arXiv, DBLP, Google Scholar, ACL Anthology, OpenReview, CVF, ACM, and IEEE Xplore, followed by backward and forward citation tracing from recent surveys and representative benchmark papers.

## 📑 Table of Contents

- [🌟 Overview](#-overview)
- [🧭 Survey Snapshot](#-survey-snapshot)
- [🔍 Key Categories](#-key-categories)
- [📚 Paper List](#-paper-list)
  - [🎯 Fundamental Competencies](#-fundamental-competencies)
  - [🧠 Higher-Order Intelligence](#-higher-order-intelligence)
  - [🌍 Real-World Applications](#-real-world-applications)
- [🚧 Emerging Directions](#-emerging-directions)
- [🤝 Contributing](#-contributing)

## 🧭 Survey Snapshot

### Corpus Snapshot

The May 2025 corpus snapshot used for the manuscript's distribution figures contains a modest number of early papers before 2022, followed by 4 papers in 2022, 10 in 2023, 41 in 2024, and 22 papers collected by May 2025. The snapshot is intended as a visual analysis slice rather than a final census of the field.

### Representative Benchmark Snapshot

The manuscript also reports a June 2026 benchmark snapshot for positioning representative benchmark families. Citation counts are used only as a rough adoption signal.

| Benchmark | Year | Evaluation Aspects | Criterion | Reported Leading Model / Score | Citations (Jun. 2026: total / since 2026) |
|---|---:|---|---|---|---:|
| MathVista | 2023 | Math | Accuracy | Qwen-2.5-VL / 74.8 | 1728 / 601 |
| MathVision | 2024 | Math | Accuracy | Gemini-2.5-Pro / 73.3 | 650 / 289 |
| UrbanVideo-Bench | 2025 | Video, embodied recall, perception, reasoning, navigation | Avg. Accuracy | Qwen-VL-Max / 45.5 | 47 / 23 |
| AgentClinic | 2024 | Clinic | Accuracy | O1-Preview / 80.0 | 238 / 92 |
| MM-SafetyBench | 2024 | Safety | Refusal Rate | - | 367 / 134 |
| OmniMedVQA | 2024 | Medical recognition, disease diagnosis, etc. | Accuracy | BLIP-2 / 50.69 | 261 / 106 |
| ProteinBench | 2024 | Protein, inverse folding, sequence design, etc. | Accuracy, functionality, etc. | ProteinMPNN / - | 31 / 10 |
| LongVideoBench | 2024 | Video, reasoning | Accuracy | GPT-4o / 66.7 | 559 / 292 |

### Case Study

The current manuscript includes a Qwen-2.5-Omni case study to show how one omni-modal model report can be mapped into the hierarchy: text, vision, audio, video, and speech-generation evaluations at the fundamental level; cross-modal reasoning and streaming response generation at the higher-order level; and deployment-oriented considerations such as robustness, latency, safety, and domain validation at the application level.

## 🔍 Key Categories

| Level | Category | Description |
|---|---|---|
| **🎯 Fundamental Competencies** | Single-modality understanding and cross-modality alignment | Core perception, comprehension, and semantic alignment across text, image, audio, video, and other modalities |
| **🧠 Higher-Order Intelligence** | Reasoning, streaming understanding, decision-making, and planning | Advanced capabilities that require temporal modeling, logical inference, tool use, state maintenance, and executable plans |
| **🌍 Real-World Applications** | Value alignment, medical, biological, industrial, and societal evaluation | Deployment-oriented benchmarks that test robustness, trustworthiness, fairness, domain expertise, and social impact |

### Subcategories

- **📷 Single Modality Understanding**: textual, visual, auditory, and other modality-specific comprehension.
- **🔗 Cross-Modality Alignment**: semantic consistency and temporal alignment across modalities.
- **💡 Multimodal Reasoning**: logical, mathematical, spatial, causal, and process-level reasoning.
- **🎬 Streaming Inputs Understanding**: long-horizon video, audio-temporal, online, and event-oriented comprehension.
- **📋 Complex Decision-Making and Planning**: tool-use, embodied planning, egocentric planning, and multi-agent coordination.
- **⚖️ Value Alignment**: instruction following, human preference alignment, safety, and adversarial robustness.
- **🏥 Medical Applications**: clinical expertise, multi-specialty generalization, fairness, hallucination, and patient-centered reliability.
- **🧬 Biological Applications**: multi-omics, protein, RNA, DNA, and drug-response evaluation.
- **🏭 Other Applications**: robotics, anomaly detection, engineering documents, transportation, agriculture, accessibility, and social-good evaluation.

## 📚 Paper List

### 🎯 Fundamental Competencies

#### 📷 Single Modality Understanding

- **[Measuring Massive Multitask Language Understanding](https://arxiv.org/abs/2009.03300)** (*2021*) `ICLR`
- **[MMLU-Pro: A More Robust and Challenging Multi-Task Language Understanding Benchmark](https://arxiv.org/abs/2406.01574)** (*2024*) `NeurIPS`
- **[CMMLU: Measuring Massive Multitask Language Understanding in Chinese](https://aclanthology.org/2024.findings-acl.671/)** (*2024*) `ACL Findings`
- **[KMMLU: Measuring Massive Multitask Language Understanding in Korean](https://aclanthology.org/2025.naacl-long.206/)** (*2025*) `NAACL`
- **[Global MMLU: Understanding and Addressing Cultural and Linguistic Biases in Multilingual Evaluation](https://aclanthology.org/2025.acl-long.919/)** (*2025*) `ACL`
- **[MMLU-ProX: A Multilingual Benchmark for Advanced Large Language Model Evaluation](https://aclanthology.org/2025.emnlp-main.79/)** (*2025*) `EMNLP`
- **[Microsoft COCO: Common Objects in Context](https://arxiv.org/abs/1405.0312)** (*2014*) `ECCV`
- **[Flickr30k Entities: Collecting Region-to-Phrase Correspondences for Richer Image-to-Sentence Models](https://openaccess.thecvf.com/content_iccv_2015/html/Plummer_Flickr30k_Entities_Collecting_ICCV_2015_paper.html)** (*2015*) `ICCV`
- **[LLaVA-Grounding: Grounded Visual Chat with Large Multimodal Models](https://arxiv.org/abs/2312.02949)** (*2024*) `ECCV`
- **[MMIU: Multimodal Multi-Image Understanding for Evaluating Large Vision-Language Models](https://arxiv.org/abs/2408.02718)** (*2025*) `ICLR`
- **[MileBench: Benchmarking MLLMs in Long Context](https://arxiv.org/abs/2404.18532)** (*2024*) `COLM`
- **[MLLM-CompBench: A Comparative Reasoning Benchmark for Multimodal LLMs](https://arxiv.org/abs/2407.16837)** (*2024*) `NeurIPS`
- **[Dynamic-SUPERB: Towards a Dynamic, Collaborative, and Comprehensive Instruction-Tuning Benchmark for Speech](https://arxiv.org/abs/2309.09510)** (*2024*) `ICASSP`
- **[MuChoMusic: Evaluating Music Understanding in Multimodal Audio-Language Models](https://arxiv.org/abs/2408.01337)** (*2024*) `ISMIR`
- **[Enabling Auditory Large Language Models for Automatic Speech Quality Evaluation](https://arxiv.org/abs/2409.16644)** (*2025*) `ICASSP`
- **[AudioBench: A Universal Benchmark for Audio Large Language Models](https://aclanthology.org/2025.naacl-long.218/)** (*2025*) `NAACL`

#### 🔗 Cross-Modality Alignment

- **[Synthesize, Diagnose, and Optimize: Towards Fine-Grained Vision-Language Understanding](https://openaccess.thecvf.com/content/CVPR2024/papers/Peng_Synthesize_Diagnose_and_Optimize_Towards_Fine-Grained_Vision-Language_Understanding_CVPR_2024_paper.pdf)** (*2024*) `CVPR`
- **[VALSE: A Task-Independent Benchmark for Vision and Language Models Centered on Linguistic Phenomena](https://aclanthology.org/2022.acl-long.567/)** (*2022*) `ACL`
- **[AudioTime: A Temporally-Aligned Audio-Text Benchmark Dataset](https://arxiv.org/abs/2407.02857)** (*2025*) `ICASSP`
- **[Simple and Controllable Music Generation](https://arxiv.org/abs/2306.05284)** (*2023*) `NeurIPS`
- **[VBench: Comprehensive Benchmark Suite for Video Generative Models](https://openaccess.thecvf.com/content/CVPR2024/papers/Huang_VBench_Comprehensive_Benchmark_Suite_for_Video_Generative_Models_CVPR_2024_paper.pdf)** (*2024*) `CVPR`
- **[Animal-Bench: Benchmarking Multimodal Video Models for Animal-Centric Video Understanding](https://proceedings.neurips.cc/paper_files/paper/2024/hash/8fa604a81e5a236e2f38e917109571a3-Abstract-Conference.html)** (*2024*) `NeurIPS`
- **[ChronoMagic-Bench: A Benchmark for Metamorphic Evaluation of Text-to-Time-Lapse Video Generation](https://arxiv.org/abs/2406.18522)** (*2024*) `NeurIPS`
- **[MME-Unify: A Comprehensive Benchmark for Unified Multimodal Understanding and Generation Models](https://openreview.net/forum?id=7x6TxVIarj)** (*2026*) `ICLR`

### 🧠 Higher-Order Intelligence

#### 💡 Multimodal Reasoning

- **[CLEVR: A Diagnostic Dataset for Compositional Language and Elementary Visual Reasoning](https://arxiv.org/abs/1612.06890)** (*2017*) `CVPR`
- **[A-OKVQA: A Benchmark for Visual Question Answering Using World Knowledge](https://arxiv.org/abs/2206.01718)** (*2022*) `ECCV`
- **[ScienceQA: Learn to Explain Multimodal Reasoning via Chain-of-Thought](https://arxiv.org/abs/2209.09513)** (*2022*) `NeurIPS`
- **[LlamaV-o1: Rethinking Step-by-Step Visual Reasoning in LLMs](https://aclanthology.org/2025.findings-acl.1247/)** (*2025*) `ACL Findings`
- **[VisuLogic: A Benchmark for Evaluating Visual Reasoning in Multi-modal Large Language Models](https://openreview.net/forum?id=mXuzDDVXxi)** (*2026*) `ICLR`
- **[X-Reasoner: Towards Generalizable Reasoning Across Modalities and Domains](https://arxiv.org/abs/2505.03981)** (*2025*) `arXiv`
- **[MathVista: Evaluating Mathematical Reasoning of Foundation Models in Visual Contexts](https://arxiv.org/abs/2310.02255)** (*2024*) `ICLR`
- **[MATH-Vision: Measuring Multimodal Mathematical Reasoning with MATH-Vision Dataset](https://doi.org/10.52202/079017-3014)** (*2024*) `NeurIPS`
- **[MathVerse: Does Your Multi-modal LLM Truly See the Diagrams in Visual Math Problems?](https://arxiv.org/abs/2403.14624)** (*2024*) `ECCV`
- **[GeomVerse: A Systematic Evaluation of Large Models for Geometric Reasoning](https://arxiv.org/abs/2312.12241)** (*2023*) `arXiv`
- **[Thinking in Space: How Multimodal Large Language Models See, Remember, and Recall Spaces](https://arxiv.org/abs/2412.14171)** (*2025*) `CVPR`
- **[LLaVA-ST: A Multimodal Large Language Model for Fine-Grained Spatial-Temporal Understanding](https://arxiv.org/abs/2501.08282)** (*2025*) `CVPR`
- **[Integrating Chain-of-Thought for Multimodal Alignment: A Study on 3D Vision-Language Learning](https://arxiv.org/abs/2503.06232)** (*2025*) `arXiv`
- **[CMMCoT: Enhancing Complex Multi-Image Comprehension via Multi-Modal Chain-of-Thought and Memory Augmentation](https://arxiv.org/abs/2503.05255)** (*2026*) `AAAI`
- **[EchoInk-R1: Exploring Audio-Visual Reasoning in Multimodal LLMs via Reinforcement Learning](https://arxiv.org/abs/2505.04623)** (*2025*) `arXiv`
- **[Exploring the Effect of Reinforcement Learning on Video Understanding: Insights from SEED-Bench-R1](https://arxiv.org/abs/2503.24376)** (*2025*) `arXiv`
- **[Reason-RFT: Reinforcement Fine-Tuning for Visual Reasoning of Vision Language Models](https://arxiv.org/abs/2503.20752)** (*2025*) `NeurIPS`

#### 🎬 Streaming Inputs Understanding

- **[TimeChat: A Time-Sensitive Multimodal Large Language Model for Long Video Understanding](https://arxiv.org/abs/2312.02051)** (*2024*) `CVPR`
- **[CinePile: A Long Video Question Answering Dataset and Benchmark](https://arxiv.org/abs/2405.08813)** (*2024*) `arXiv`
- **[LongVideoBench: A Benchmark for Long-Context Interleaved Video-Language Understanding](https://arxiv.org/abs/2407.15754)** (*2024*) `arXiv`
- **[EgoSchema: A Diagnostic Benchmark for Very Long-Form Video Language Understanding](https://arxiv.org/abs/2308.09126)** (*2023*) `NeurIPS`
- **[EAGLE: Egocentric AGgregated Language-Video Engine](https://arxiv.org/abs/2409.17523)** (*2024*) `ACM MM`
- **[ViLMA: A Zero-Shot Benchmark for Linguistic and Temporal Grounding in Video-Language Models](https://arxiv.org/abs/2311.07022)** (*2024*) `ICLR`
- **[VITATECS: A Diagnostic Dataset for Temporal Concept Understanding of Video-Language Models](https://arxiv.org/abs/2311.17404)** (*2024*) `ECCV`
- **[OSCaR: Object State Captioning and State Change Representation](https://aclanthology.org/2024.findings-naacl.226/)** (*2024*) `NAACL Findings`
- **[STAR: A Benchmark for Situated Reasoning in Real-World Videos](https://datasets-benchmarks-proceedings.neurips.cc/paper_files/paper/2021/hash/5ef059938ba799aaa845e1c2e8a762bd-Abstract-round2.html)** (*2021*) `NeurIPS Datasets and Benchmarks`
- **[V-STaR: Benchmarking Video-LLMs on Video Spatio-Temporal Reasoning](https://arxiv.org/abs/2503.11495)** (*2026*) `CVPR Findings`
- **[AIR-Bench: Benchmarking Large Audio-Language Models via Generative Comprehension](https://aclanthology.org/2024.acl-long.109/)** (*2024*) `ACL`
- **[DAVE: Diagnostic Benchmark for Audio Visual Evaluation](https://arxiv.org/abs/2503.09321)** (*2025*) `NeurIPS Datasets and Benchmarks`
- **[TempCompass: Do Video LLMs Really Understand Videos?](https://aclanthology.org/2024.findings-acl.517/)** (*2024*) `ACL Findings`
- **[OVO-Bench: How Far is Your Video-LLMs from Real-World Online Video Understanding?](https://arxiv.org/abs/2501.05510)** (*2025*) `CVPR`
- **[AutoEval-Video: An Automatic Benchmark for Assessing Large Vision Language Models in Open-Ended Video Question Answering](https://arxiv.org/abs/2311.14906)** (*2024*) `ECCV`
- **[ALLVB: All-in-One Long Video Understanding Benchmark](https://arxiv.org/abs/2503.07298)** (*2025*) `AAAI`
- **[UrbanVideo-Bench: Benchmarking Vision-Language Models on Embodied Intelligence with Video Data in Urban Spaces](https://aclanthology.org/2025.acl-long.1558/)** (*2025*) `ACL`
- **[MMWorld: Towards Multi-Discipline Multi-Faceted World Model Evaluation in Videos](https://openreview.net/forum?id=mDRmX8IlBI)** (*2025*) `ICLR`
- **[WorldSense: Evaluating Real-World Omnimodal Understanding for Multimodal LLMs](https://openreview.net/forum?id=YxsfxAvJv4)** (*2026*) `ICLR`
- **[EventBench: Towards Event-Oriented Long Video Understanding](https://arxiv.org/abs/2406.14129)** (*2024*) `arXiv`

#### 📋 Complex Decision-Making and Planning

- **[m&m's: A Benchmark to Evaluate Tool-Use for Multi-Step Multi-Modal Tasks](https://doi.org/10.1007/978-3-031-72684-2_2)** (*2024*) `ECCV`
- **[AgentClinic: A Multimodal Benchmark for Tool-Using Clinical AI Agents](https://doi.org/10.1038/s41746-026-02674-7)** (*2026*) `npj Digital Medicine`
- **[MuEP: A Multimodal Benchmark for Embodied Planning with Foundation Models](https://www.ijcai.org/proceedings/2024/15)** (*2024*) `IJCAI`
- **[MFE-ETP: A Comprehensive Evaluation Benchmark for Multi-Modal Foundation Models on Embodied Task Planning](https://arxiv.org/abs/2407.05047)** (*2024*) `arXiv`
- **[EgoPlan-Bench: Benchmarking Multimodal Large Language Models for Human-Level Planning](https://doi.org/10.1007/s11263-025-02676-0)** (*2026*) `IJCV`
- **[EgoPlan-Bench2: A Benchmark for Multimodal Large Language Model Planning in Real-World Scenarios](https://doi.org/10.1007/s11263-026-02826-y)** (*2026*) `IJCV`
- **[Sampling-Based Multi-Modal Multi-Robot Multi-Goal Path Planning](https://arxiv.org/abs/2503.03509)** (*2026*) `arXiv`

### 🌍 Real-World Applications

#### ⚖️ Value Alignment

- **[Visual Instruction Tuning](https://proceedings.neurips.cc/paper_files/paper/2023/file/6dcf277ea32ce3288914faf369fe6de0-Paper-Conference.pdf)** (*2023*) `NeurIPS`
- **[LLaVA-NeXT: Stronger LLMs Supercharge Multimodal Capabilities in the Wild](https://llava-vl.github.io/blog/2024-05-10-llava-next-stronger-llms/)** (*2024*) `Project`
- **[MIA-Bench: Towards Better Instruction Following Evaluation of Multimodal LLMs](https://openreview.net/forum?id=7EhS3YBxjY)** (*2025*) `ICLR`
- **[MM-IFEngine: Towards Multimodal Instruction Following](https://openaccess.thecvf.com/content/ICCV2025/html/Ding_MM-IFEngine_Towards_Multimodal_Instruction_Following_ICCV_2025_paper.html)** (*2025*) `ICCV`
- **[The Multimodal Arena is Here!](https://lmsys.org/blog/2024-06-27-multimodal/)** (*2024*) `Project`
- **[WildVision: Evaluating Vision-Language Models in the Wild with Human Preferences](http://papers.nips.cc/paper_files/paper/2024/hash/563991b5c8b45fe75bea42db738223b2-Abstract-Datasets_and_Benchmarks_Track.html)** (*2024*) `NeurIPS`
- **[OmniAlign-V: Towards Enhanced Alignment of MLLMs with Human Preference](https://aclanthology.org/2025.acl-long.906/)** (*2025*) `ACL`
- **[Align Anything: Training All-Modality Models to Follow Instructions with Language Feedback](https://doi.org/10.48550/arXiv.2412.15838)** (*2024*) `arXiv`
- **[MM-SafetyBench: A Benchmark for Safety Evaluation of Multimodal Large Language Models](https://doi.org/10.1007/978-3-031-72992-8_22)** (*2024*) `ECCV`
- **[MM-RLHF: The Next Step Forward in Multimodal LLM Alignment](https://arxiv.org/abs/2502.10391)** (*2025*) `ICML`
- **[B-AVIBench: Toward Evaluating the Robustness of Large Vision-Language Model on Black-Box Adversarial Visual-Instructions](https://doi.org/10.1109/TIFS.2024.3520306)** (*2025*) `TIFS`
- **[AVTrustBench: Assessing and Enhancing Reliability and Robustness in Audio-Visual LLMs](https://doi.org/10.48550/arXiv.2501.02135)** (*2025*) `ICCV`

#### 🏥 Medical Applications

- **[RJUA-MedDQA: A Multimodal Benchmark for Medical Document Question Answering and Clinical Reasoning](https://doi.org/10.1145/3637528.3671644)** (*2024*) `KDD`
- **[MedXpertQA: Benchmarking Expert-Level Medical Reasoning and Understanding](https://proceedings.mlr.press/v267/zuo25a.html)** (*2025*) `ICML`
- **[Asclepius: A Spectrum Evaluation Benchmark for Medical Multi-Modal Large Language Models](https://aclanthology.org/2025.acl-long.1178/)** (*2025*) `ACL`
- **[OmniMedVQA: A New Large-Scale Comprehensive Evaluation Benchmark for Medical LVLM](https://arxiv.org/abs/2402.09181)** (*2024*) `CVPR`
- **[GMAI-MMBench: A Comprehensive Multimodal Evaluation Benchmark Towards General Medical AI](https://arxiv.org/abs/2408.03361)** (*2024*) `NeurIPS`
- **[MMIST-ccRCC: A Real World Medical Dataset for the Development of Multi-Modal Systems](https://openaccess.thecvf.com/content/CVPR2024W/DCAMI/papers/Mota_MMIST-ccRCC_A_Real_World_Medical_Dataset_for_the_Development_of_CVPRW_2024_paper.pdf)** (*2024*) `CVPR Workshop`
- **[Touchstone Benchmark: Are We on the Right Way for Evaluating AI Algorithms for Medical Segmentation?](https://doi.org/10.52202/079017-0485)** (*2024*) `NeurIPS`
- **[BenchX: A Unified Benchmark Framework for Medical Vision-Language Pretraining on Chest X-Rays](https://doi.org/10.52202/079017-0213)** (*2024*) `NeurIPS`
- **[MultiMedEval: A Benchmark and a Toolkit for Evaluating Medical Vision-Language Models](https://arxiv.org/abs/2402.09262)** (*2024*) `MIDL`
- **[3MDBench: Medical Multimodal Multi-Agent Dialogue Benchmark](https://aclanthology.org/2025.emnlp-main.1353/)** (*2025*) `EMNLP`
- **[FMBench: Benchmarking Fairness in Multimodal Large Language Models on Medical Tasks](https://arxiv.org/abs/2410.01089)** (*2024*) `arXiv`
- **[FairMedFM: Fairness Benchmarking for Medical Imaging Foundation Models](https://doi.org/10.52202/079017-3535)** (*2024*) `NeurIPS`
- **[MediConfusion: Can You Trust Your AI Radiologist?](https://openreview.net/forum?id=H9UnNgdq0g)** (*2025*) `ICLR`
- **[MedHallBench: A New Benchmark for Assessing Hallucination in Medical Large Language Models](https://proceedings.mlr.press/v281/zuo25b.html)** (*2025*) `PMLR`

#### 🧬 Biological Applications

- **[scDrugMap: Benchmarking Large Foundation Models for Drug Response Prediction](https://arxiv.org/abs/2505.05612)** (*2025*) `arXiv`
- **[ProteinBench: A Holistic Evaluation of Protein Foundation Models](https://arxiv.org/abs/2409.06744)** (*2024*) `ICLR`
- **[A Fine-Tuning Dataset and Benchmark for Large Language Models for Protein Understanding](https://arxiv.org/abs/2406.05540)** (*2024*) `BIBM`
- **[Prot2Text: Multimodal Protein's Function Generation with GNNs and Transformers](https://arxiv.org/abs/2307.14367)** (*2024*) `AAAI`
- **[Bridging Sequence-Structure Alignment in RNA Foundation Models](https://arxiv.org/abs/2407.11242)** (*2025*) `AAAI`
- **[DRFormer: A Benchmark Model for RNA Sequence Downstream Tasks](https://www.mdpi.com/2073-4425/16/3/284)** (*2025*) `Genes`
- **[BEACON: Benchmark for Comprehensive RNA Tasks and Language Models](https://arxiv.org/abs/2406.10391)** (*2024*) `NeurIPS`
- **[BEND: Benchmarking DNA Language Models on Biologically Meaningful Tasks](https://arxiv.org/abs/2311.12570)** (*2024*) `ICLR`
- **[GenBench: A Benchmarking Suite for Systematic Evaluation of Genomic Foundation Models](https://arxiv.org/abs/2406.01627)** (*2024*) `arXiv`
- **[A Benchmark Dataset for Multimodal Prediction of Enzymatic Function Coupling DNA Sequences and Natural Language](https://arxiv.org/abs/2407.15888)** (*2024*) `arXiv`

#### 🏭 Other Applications

- **[Coordinating Hundreds of Cooperative, Autonomous Vehicles in Warehouses](https://doi.org/10.1609/aimag.v29i1.2082)** (*2008*) `AI Magazine`
- **[MMRo: Are Multimodal LLMs Eligible as the Brain for In-Home Robotics?](https://arxiv.org/abs/2406.19693)** (*2024*) `arXiv`
- **[Deep Learning-Based Defect Detection of Metal Parts: Evaluating Current Methods in Complex Conditions](https://doi.org/10.1109/ICUMT54235.2021.9631567)** (*2021*) `ICUMT`
- **[MVTec AD: A Comprehensive Real-World Dataset for Unsupervised Anomaly Detection](https://openaccess.thecvf.com/content_CVPR_2019/html/Bergmann_MVTec_AD_--_A_Comprehensive_Real-World_Dataset_for_Unsupervised_Anomaly_CVPR_2019_paper.html)** (*2019*) `CVPR`
- **[MMAD: A Comprehensive Benchmark for Multimodal Large Language Models in Industrial Anomaly Detection](https://arxiv.org/abs/2410.09453)** (*2025*) `ICLR`
- **[DesignQA: A Multimodal Benchmark for Evaluating Large Language Models' Understanding of Engineering Documentation](https://doi.org/10.1115/1.4067333)** (*2025*) `JCISE`
- **[MME-Industry: A Cross-Industry Multimodal Evaluation Benchmark](https://arxiv.org/abs/2501.16688)** (*2025*) `arXiv`
- **[TransportationGames: Benchmarking Transportation Knowledge of (Multimodal) Large Language Models](https://arxiv.org/abs/2401.04471)** (*2024*) `arXiv`
- **[MM-SOC: Benchmarking Multimodal Large Language Models in Social Media Platforms](https://aclanthology.org/2024.findings-acl.370/)** (*2024*) `ACL Findings`
- **[AgriBench: A Hierarchical Agriculture Benchmark for Multimodal Large Language Models](https://doi.org/10.1007/978-3-031-91835-3_14)** (*2025*) `ECCV Workshop`
- **[AgMMU: A Comprehensive Agricultural Multimodal Understanding Benchmark](https://openreview.net/forum?id=MQPZPtv8GG)** (*2025*) `NeurIPS`
- **[VizWiz Grand Challenge: Answering Visual Questions from Blind People](https://openaccess.thecvf.com/content_cvpr_2018/html/Gurari_VizWiz_Grand_Challenge_CVPR_2018_paper.html)** (*2018*) `CVPR`
- **[Vision-Braille: A Curriculum Learning Toolkit and Braille-Chinese Corpus for Braille Translation](https://arxiv.org/abs/2407.06048)** (*2026*) `arXiv`

## 🚧 Emerging Directions

The manuscript highlights several directions where evaluation practice still needs stronger benchmarks and protocols:

- **Multilingual multimodal evaluation**: [PM4Bench](https://arxiv.org/abs/2503.18484), [M4U](https://openaccess.thecvf.com/content/WACV2026/papers/Wang_M4U_Evaluating_Multilingual_Understanding_and_Reasoning_for_Large_Multimodal_Models_WACV_2026_paper.pdf), [M5](https://aclanthology.org/2024.findings-emnlp.250/), and [xGQA](https://aclanthology.org/2022.findings-acl.196/) show that language ability, OCR, culture, and safety are difficult to disentangle.
- **Interactive and embodied benchmarks**: [AVLEN](https://doi.org/10.52202/068431-0451), [ELBA](https://openaccess.thecvf.com/content/WACV2025/html/Shen_ELBA_Learning_by_Asking_for_Embodied_Visual_Navigation_and_Task_WACV_2025_paper.html), [LEO](https://proceedings.mlr.press/v235/huang24ae.html), and [3DLLM-Mem](https://proceedings.neurips.cc/paper_files/paper/2025/hash/61f527a737e4ba61f3e10d6c3f0c4b55-Abstract-Conference.html) move evaluation toward feedback, memory, and embodied action.
- **Auto-evaluation vs. human-in-the-loop trade-offs**: [LAVE](https://ojs.aaai.org/index.php/AAAI/article/view/28212) and [MM-Vet](https://proceedings.mlr.press/v235/yu24o.html) illustrate the need to balance scalable automatic scoring with human judgment for open-ended multimodal outputs.

## 🤝 Contributing

Contributions are welcome. Please open a Pull Request with the paper title, venue or preprint status, year, link, and the most appropriate taxonomy category.
