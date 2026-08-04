# Awesome-Computational-Pathology-Papers

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

> *Last updated: Jun 2025*

If you find this repository useful, please consider  **giving us a star** 🌟

## 💡 Background
Computational pathology combines advanced imaging techniques, deep learning algorithms, and multimodal data integration to transform traditional histopathology workflows into quantitative, scalable, and precision-oriented practices. 
This repository collects state-of-the-art papers (most from Nature family journals, Cell Press, Science family journals, and some top-tier conferences) highlighting significant progress in pathology foundation models, multimodal generative AI, virtual staining methods, biomarker prediction, and clinical translation. These works not only drive forward precision oncology and personalized medicine but also address fundamental challenges such as model generalizability, interpretability, demographic bias, and ethical implications, reflecting the rapidly evolving landscape of AI-driven digital pathology.

---
## 📖 Awesome list criteria

---
## 🗂️ Contents
- [Foundation Models & Feature Engineering](#1--pathology--biomedical-foundation-models--feature-engineering)
- [Generative Models & Virtual Staining](#2--generative-models--virtual-staining)
- [Multimodal LLMs & Reasoning](#3--multimodal-llms-mllm--reasoning)
- [Datasets & Benchmarks](#4--datasets--benchmarks)
- [Clinical Applications & Biomarker Prediction](#5--clinical-applications--biomarker-prediction)
- [3D / Spatial-Omics & Multimodal Imaging](#6--3d--spatial-omics--multimodal-imaging)
- [Methodology, Algorithms & Bias](#7--methodology-algorithms--bias)
- [Reviews, Surveys & Perspectives](#8--reviews-surveys--perspectives)

---

## 1. Pathology & Biomedical **Foundation Models / Feature-Engineering**

| Paper                                                                                 | Venue               | Date         | Highlight                                              | Links |
| ------------------------------------------------------------------------------------- | ------------------- | ------------ | ------------------------------------------------------ | ----- |
| UniBiomed: A Universal Foundation Model for Grounded Biomedical Image Interpretation  | *arXiv*             | **Jun 2025** | Cross-modal FM covering 9 imaging modalities           |[[PDF]](https://arxiv.org/pdf/2504.21336?)|
| A multimodal vision foundation model for clinical dermatology                         | *Nat. Med.*         | **Jun 2025** | Skin-imaging FM with dermatology benchmarks            |[[PDF]](https://www.nature.com/articles/s41591-025-03747-y.pdf)|
| A foundation model for generalizable cancer diagnosis & survival prediction           | *Nat. Commun.*      | **Apr 2025** | End-to-end prognosis from WSIs                         |[[PDF]](https://www.nature.com/articles/s41467-025-57587-y.pdf)|
| Towards A Generalizable Pathology Foundation Model via Unified Knowledge Distillation | *Nat. Biomed. Eng.* | **Apr 2025** | Knowledge-distilled FM that transfers across cohorts   |       |
| Foundation models for fast, label-free detection of glioma infiltration               | *Nature*            | **Feb 2025** | Intra-operative FM enabling real-time tumor margining  |       |
| Exploring Scalable Medical Image Encoders Beyond Text Supervision                     | *arXiv*             | **Feb 2025** | Large-scale SSL encoders for medical images            |       |
| Molecular-driven Foundation Model for Oncologic Pathology                             | *arXiv*             | **Jan 2025** | Incorporates genomics into pathology FM pre-training   |       |
| A pathology foundation model for cancer diagnosis & prognosis prediction              | *Nature*            | **Oct 2024** | WSI FM evaluated on 20 cancer types                    |       |
| Multimodal Whole-Slide Foundation Model for Pathology                                 | *arXiv*             | **Nov 2024** | Joint image–text pre-training on >10 M WSI patches     |       |
| A foundation model for enhancing MR images & downstream tasks                         | *Nat. Biomed. Eng.* | **Oct 2024** | Diffusion-based super-resolution FM for MRI            |       |
| Mapping histomorphological cancer phenotypes via self-supervised learning             | *Nat. Commun.*      | **Jun 2024** | No-label SSL on 2.5 M slides                           |       |
| A foundation model for clinical-grade computational pathology & rare-cancer detection | *Nat. Med.*         | **Jun 2024** | Out-of-distribution detection of <2% incidence cancers |       |
| A whole-slide foundation model from real-world data                                   | *Nature*            | **Jun 2024** | 5-B-parameter FM pre-trained on hospital WSIs          |       |
| RudolfV: A Foundation Model by Pathologists for Pathologists                          | *arXiv*             | **Jan 2024** | Expert-curated pre-training corpus                     |       |

---

## 2. **Generative Models & Virtual Staining**

| Paper                                                                               | Venue               | Date         | Highlight                                                   | Links |
| ----------------------------------------------------------------------------------- | ------------------- | ------------ | ----------------------------------------------------------- | ----- |
| PixCell: A Generative Foundation Model for Digital Histopathology Images            | *arXiv*             | **Jun 2025** | Diffusion FM producing 16k×16k virtual WSIs                 |       |
| Pixel super-resolved virtual staining of label-free tissue using diffusion models   | *Nat. Commun.*      | **Jun 2025** | Sub-micron resolution synthetic stains                      |       |
| Self-improving generative foundation model for synthetic medical image generation   | *Nat. Med.*         | **Feb 2025** | Continual learning diffusion FM                             |       |
| Generation of synthetic WSI tiles from RNA-seq via cascaded diffusion models        | *Nat. Biomed. Eng.* | **Mar 2025** | Transcriptome → histology synthesis                         |       |
| Learned representation-guided diffusion models for large-image generation           | *CVPR*              | **Jun 2024** | Generates giga-pixel imagery with memory-efficient sampling |       |
| A multimodal generative AI copilot for human pathology                              | *Nature*            | **Jun 2024** | Image-conditioned text generation for reporting             |       |
| Generative models improve fairness of medical classifiers under distribution shifts | *Nat. Med.*         | **Apr 2024** | Data augmentation for bias mitigation                       |       |
| Virtual histological staining of unlabeled autopsy tissue                           | *Nat. Commun.*      | **Mar 2024** | First virtual staining study on post-mortem tissue          |       |

---

## 3. **Multimodal LLMs (MLLM) & Reasoning**

| Paper                                                                                 | Venue          | Date         | Highlight                                          | Links |
| ------------------------------------------------------------------------------------- | -------------- | ------------ | -------------------------------------------------- | ----- |
| Patho-R1: A Multimodal Reinforcement Learning-Based Pathology Expert Reasoner         | *arXiv*        | **May 2025** | RL-tuned agent that asks & answers slide questions |       |
| ChestX-Reasoner: Advancing Radiology Foundation Models with Step-by-Step Verification | *arXiv*        | **May 2025** | Chain-of-thought verification for chest CT         |       |
| VisualPRM: An Effective Process Reward Model for Multimodal Reasoning                 | *arXiv*        | **Mar 2025** | Reward-shaping for V-L reasoning tasks             |       |
| InternVL3: Training & Test-time Recipes for Open-Source MMLMs                         | *Tech report*  | **Apr 2025** | Tricks for scaling to 4096 × 4096 inputs           |       |
| Mini-InternVL: 5 % Params, 90 % Performance                                           | *Tech report*  | **Nov 2024** | Lightweight MLLM for edge deployment               |       |
| In-context learning enables MLLMs to classify cancer pathology images                 | *Nat. Commun.* | **Aug 2024** | Zero-shot WSI classification via ICL               |       |
| looongLLaVA: Scaling MLLMs to 1000 Images Efficiently                                 | *arXiv*        | **Sep 2024** | Hybrid visual memory for ultra-long contexts       |       |
| Quilt-LLaVA: Instruction Tuning from Histopathology Videos                            | *CVPR*         | **Jun 2024** | Localized narrative extraction for slide QA        |       |
| SlideChat: A Large V-L Assistant for Whole-Slide Images                               | *CVPR*         | **Oct 2024** | Dialogue-centric WSI agent with 400 k Q–A pairs    |       |
| Advancing Multimodal Medical Capabilities of Gemini                                   | *Tech report*  | **May 2024** | Google Gemini medical evaluation                   |       |
| HuatuoGPT-Vision: Injecting Medical Visual Knowledge into MLLMs                       | *EMNLP*        | **Sep 2024** | Bilingual (CN-EN) medical-vision MLLM              |       |
| A Foundational Multimodal Vision-Language AI Assistant for Human Pathology            | *arXiv*        | **Dec 2023** | Early large-scale slide chatbot                    |       |
| A Multimodal Knowledge-enhanced Whole-Slide Pathology FM                              | *arXiv*        | **Aug 2024** | Knowledge graph joins vision tokens                |       |
| Vision–language foundation model for precision oncology                               | *Nature*       | **Feb 2025** | V-L FM predicts biomarkers & therapy response      |       |

---

## 4. **Datasets & Benchmarks**

| Paper                                                                           | Venue          | Date         | Highlight                                | Links |
| ------------------------------------------------------------------------------- | -------------- | ------------ | ---------------------------------------- | ----- |
| TCGA virtual spatial transcriptomics atlas | *medRxiv* | **2026** | DeepSpot-M predicted ST for ~28.7k TCGA H&E slides | [[HF]](https://huggingface.co/datasets/ratschlab/TCGA_virtual_spatial_transcriptomics_atlas) [[PDF]](https://www.medrxiv.org/content/10.64898/2026.06.19.26356060v1) [[Code]](https://github.com/ratschlab/DeepSpotM) |
| HEST Xenium virtual spatial transcriptomics | *medRxiv* | **2026** | DeepSpot-M predicted ST for 59 HEST Xenium samples (~13.3M cells) | [[HF]](https://huggingface.co/datasets/ratschlab/HEST_Xenium_virtual_spatial_transcriptomics) [[PDF]](https://www.medrxiv.org/content/10.64898/2026.06.19.26356060v1) [[Code]](https://github.com/ratschlab/DeepSpotM) |
| MedBookVQA: A Systematic & Comprehensive Medical VQA Benchmark                  | *arXiv*        | **Jun 2025** | 2 M Q–A pairs from open-access textbooks |       |
| PathBench: A Comparison Benchmark for Pathology Foundation Models               | *arXiv*        | **May 2025** | 12 tasks, 30 + FMs, oncology-oriented    |       |
| MEDTRINITY-25M: A Large-Scale Multimodal Dataset with Multigranular Annotations | *ICLR*         | **Feb 2025** | 25 M image-text pairs across 17 organs   |       |
| PHARAOH: A Crowdsourcing Platform for Histology Phenotyping                     | *Nat. Commun.* | **Jan 2025** | 50 k expert-verified ROI labels          |       |
| HEST-1k: A Dataset for Spatial Transcriptomics & Histology                      | *NeurIPS*      | **Dec 2024** | 1 k paired ST–WSI samples                |       |
| RadGenome-Chest CT: A Grounded V-L Dataset                                      | *arXiv*        | **Apr 2024** | Combines ROI boxes & genetic markers     |       |
| WSI-VQA: Interpreting Whole-Slide Images by Generative VQA                      | *ECCV*         | **Jul 2024** | 8 k high-res slide questions             |       |

---

## 5. **Clinical Applications & Biomarker Prediction**

| Paper                                                                               | Venue          | Date         | Highlight                              | Links |
| ----------------------------------------------------------------------------------- | -------------- | ------------ | -------------------------------------- | ----- |
| Deep learning using histological images for gene-mutation prediction in lung cancer | *The Lancet*   | **Jan 2025** | Multi-centre mutation prediction study |       |
| Prediction of recurrence risk in endometrial cancer with multimodal DL              | *Nat. Med.*    | **Jul 2024** | Combines WSI & clinical data           |       |
| Histopathologic DL classifier for platinum-response in ovarian cancer               | *Nat. Commun.* | **May 2024** | Treatment-response predictor           |       |
| Prediction of tumor origin in cancers of unknown primary                            | *Nat. Med.*    | **Apr 2024** | Cytology images beat DNA panels        |       |
| ANORAK improves histopathological grading of lung adenocarcinoma                    | *Nat. Cancer*  | **Feb 2024** | AI-augmented grading workflow          |       |
| Population-level digital histologic biomarker for breast-cancer prognosis           | *Nat. Med.*    | **Jan 2024** | 1 M patient registry validation        |       |
| A vision–language foundation model for precision oncology                           | *Nature*       | **Feb 2025** | (see FM table)                         |       |

---

## 6. **3D / Spatial-Omics & Multimodal Imaging**

| Paper                                                   | Venue            | Date         | Highlight                                     | Links |
| ------------------------------------------------------- | ---------------- | ------------ | --------------------------------------------- | ----- |
| DeepSpot2Cell: Predicting Virtual Single-Cell Spatial Transcriptomics from H&E images using Spot-Level Supervision | *NeurIPS* | **2025** | Virtual single-cell ST from H&E with spot-level supervision | [[PDF]](https://openreview.net/forum?id=ofCkwXQKaz) [[Code]](https://github.com/ratschlab/DeepSpot2Cell) |
| DeepSpot-M: a multimodal foundation model for transcriptome-wide virtual spatial transcriptomics from histology | *medRxiv* | **2026** | Transcriptome-wide virtual ST from histology tiles | [[PDF]](https://www.medrxiv.org/content/10.64898/2026.06.19.26356060v1) [[Code]](https://github.com/ratschlab/DeepSpotM) |
| DeepSpot: Leveraging Spatial Context for Enhanced Spatial Transcriptomics Prediction from H&E Images | *medRxiv* | **2025** | ST prediction from H&E with spatial context | [[PDF]](https://www.medrxiv.org/content/10.1101/2025.02.09.25321567v3) [[Code]](https://github.com/ratschlab/DeepSpot) |
| Representation learning for multi-modal spatially resolved transcriptomics data (AESTETIK) | *Bioinformatics* | **2026** | Multi-modal ST + morphology representation learning | [[PDF]](https://academic.oup.com/bioinformatics/advance-article/doi/10.1093/bioinformatics/btag316/8692433) [[Code]](https://github.com/ratschlab/aestetik) |
| AI-driven 3D Spatial Transcriptomics                    | *arXiv*          | **Feb 2025** | Generates 3-D ST volumes from serial sections |       |
| An end-to-end workflow for nondestructive 3-D pathology | *Nat. Protocols* | **Apr 2024** | Clears, images & analyses thick tissue        |       |

---

## 7. **Methodology, Algorithms & Bias**

| Paper                                                                     | Venue       | Date         | Highlight                                        | Links |
| ------------------------------------------------------------------------- | ----------- | ------------ | ------------------------------------------------ | ----- |
| Do Multiple Instance Learning Models Transfer?                            | *ICML*      | **Jun 2025** | Large-scale MIL transferability study            |       |
| Vision Transformers Need Registers                                        | *ICLR*      | **Jun 2024** | Architectural tweak boosting ViT convergence     |       |
| Demographic bias of expert-level V-L foundation models in medical imaging | *Sci. Adv.* | **Mar 2025** | Finds systematic under-performance on minorities |       |
| Demographic bias in misdiagnosis by computational pathology models        | *Nat. Med.* | **Feb 2024** | Patient-level bias audit across 4 cohorts        |       |

---

## 8. **Reviews, Surveys & Perspectives**

| Paper                                                                   | Venue                    | Date         | Highlight                                 | Links |
| ----------------------------------------------------------------------- | ------------------------ | ------------ | ----------------------------------------- | ----- |
| Artificial intelligence in digital pathology — time for a reality check | *Nat. Rev. Clin. Oncol.* | **Apr 2025** | Critical appraisal of deployment hurdles  |       |
| Foundation Models – A Panacea for AI in Pathology?                      | *arXiv*                  | **Feb 2025** | Opportunities & pitfalls of pathology FMs |       |
| Multi-Modal Foundation Models for Computational Pathology: A Survey     | *arXiv*                  | **Mar 2025** | Catalogues 60 + MLLM/FMs                  |       |
| Generative Models in Computational Pathology: A Comprehensive Survey    | *arXiv*                  | **May 2025** | End-to-end review of diffusion & GANs     |       |
| A Survey of Pathology Foundation Models: Progress & Future Directions   | *IJCAI*                  | **Apr 2025** | Taxonomy & benchmark summary              |       |
| Data-Centric Foundation Models in Computational Healthcare              | *arXiv*                  | **Nov 2024** | Argues for data-quality over model size   |       |
| A Guide to AI for Cancer Researchers                                    | *Nat. Rev. Cancer*       | **Jun 2024** | Plain-language intro for oncologists      |       |
| A New Era in Computational Pathology: Survey on FM & V-L Models         | *arXiv*                  | **Sep 2024** | Early holistic survey                     |       |
| A systematic review on MLLMs in computational pathology                 | *arXiv*                  | **Jan 2025** | Focused on slide-level V-L models         |       |
| A Clinical Benchmark of Public Self-Supervised Pathology FMs            | *Nat. Commun.*           | **Apr 2025** | Head-to-head evaluation of 15 SSL models  |       |
| Multimodal Generative AI for Medical Image Interpretation (Perspective) | *Nature*                 | **Mar 2025** | Outlook on Gen-AI regulators & ethics     |       |

---

## 🧑‍💻 Contributing
If you would like to contribute, please read the [contribution guidelines](CONTRIBUTING.md) and submit a pull request.
If you find some ignored papers, feel free to create pull requests, or open issues. Contributions in any form to make this list more comprehensive are welcome. 📣📣📣


[//]: # (## ⚖️ License)
