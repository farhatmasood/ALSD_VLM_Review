[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/farhatmasood/ALSD_VLM_Review)
[![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
![Papers](https://img.shields.io/badge/Papers-213-blue)
![Studies](https://img.shields.io/badge/Reviewed_Studies-165-orange)

# <p align=center> "Vision-Language Foundation Models for Lumbar Spine Diagnostics: A Systematic Review of Architectures, Knowledge Distillation and Clinical Deployment Pathways" </p>

<!-- Authors: [Rao Farhat Masood](https://orcid.org/0000-0001-9054-9192) and [Imtiaz Ahmad Taj](https://orcid.org/0000-0003-1813-5563)

Department of Electrical and Computer Engineering, Capital University of Science and Technology (CUST), Islamabad, Pakistan

Corresponding author: farhatmasood.fm@gmail.com -->
</p>

---

## Summary

Vision–language models (VLMs) and large language models (LLMs) are increasingly applied to medical image analysis, yet their adoption in spine diagnostics lacks systematic evaluation. This review synthesizes **165 peer-reviewed studies (2015–2026)**, presenting a unified mathematical framework for multimodal architectures spanning foundation models, knowledge distillation pipelines, volumetric processors and automated report generators. We formalize the design space through a common notation system for self-attention, contrastive pre-training and distillation losses and establish quantitative comparisons across six evaluation metrics (DSC, IoU, sensitivity, specificity, AUC, Cohen's κ). A random-effects meta-analysis of 14 spine segmentation studies yields a pooled vertebral Dice coefficient of **μ̂ = 0.897** (95% CI: 0.881–0.913; I² = 74.3%), with domain-specific models consistently surpassing general-purpose architectures. Peer-reviewed lumbar systems achieve **DSC of 0.93** on the VerSe benchmark, multi-label **IoU of 0.88** across 61 disorder combinations in 28,065 patients and stenosis detection **sensitivity of 0.93** at specificity 0.95 in blinded multi-reader studies. We introduce a spine-centric evaluation framework for more than 35 models across four architectural paradigms, present set-theoretic capability analysis and provide deployment recommendations stratified by computational constraints. Six critical research gaps are identified and a resource-stratified deployment roadmap is proposed to guide clinical translation.

---

## Highlights

- **Comprehensive scope**: Systematic review of 165 peer-reviewed studies (2015–2026) on VLMs and LLMs for automated lumbar spine diagnostics.
- **Spine-centric taxonomy**: Classification of 35+ medical LLMs and VLMs organized by architectural paradigm, multi-sequence MRI input capability and clinical deployment tier, with a role-centric matrix linking each model to specific lumbar pipeline functions.
- **Unified mathematical framework**: Formalization of self-attention, CLIP contrastive pre-training, composite spine segmentation loss and knowledge distillation objectives, together with an empirically supported specialization–generalization ordering and an information-theoretic distillation bound.
- **Meta-analytic synthesis**: Random-effects pooling of vertebral segmentation DSC across 14 spine studies (μ̂ = 0.897; 95% CI: 0.881–0.913; I² = 74.3%), with systematic heterogeneity analysis.
- **3D-aware model assessment**: Computational overhead quantification and multi-sequence MRI capability mapping for volumetric spine models.
- **Knowledge distillation analysis**: Task-stratified compression results with a unified teacher–student pipeline for clinical deployment across three resource tiers.
- **Six research gaps identified**: Absence of standardized 3D spine benchmarks, insufficient prospective validation, distillation limitations for spatial representations, hallucination risks, demographic bias in training data, and the need for explainable AI.
- **Evidence-based deployment roadmap**: Three-tier deployment recommendations (community → district → tertiary) with model-specific hardware requirements, expected DSC ranges and inference latency guidance.

---

## Study Distribution

| Research Category | MRI | CT | Total |
|---|---|---|---|
| Spine-specific diagnostic systems | 28 | 14 | 42 |
| General medical VLMs | 18 | 6 | 24 |
| Medical image segmentation | 22 | 15 | 37 |
| Report generation & clinical NLP | 12 | 3 | 15 |
| Knowledge distillation pipelines | 8 | 5 | 13 |
| Foundation model adaptation | 11 | 4 | 15 |
| Benchmark & dataset publications | 7 | 4 | 11 |
| Text-only medical LLMs | — | — | 8 |
| **Total** | | | **165** |

---

<hr />

# <p align=center>`VLMs & LLMs for Lumbar Spine Diagnostics`</p>

A curated list of all **213 references** cited in the survey, organized by category (**in chronological order within each section**). We intend to regularly update this page with the latest relevant papers.

We strongly encourage the researchers that want to promote their work to make pull requests to update their paper's information!

## Overview
- [Survey & Review Papers](#survey--review-papers)
- [Foundational Architectures & Deep Learning](#foundational-architectures--deep-learning)
- [General-Purpose Foundation Models](#general-purpose-foundation-models)
- [Medical Vision-Language Models](#medical-vision-language-models)
- [Medical Image Segmentation](#medical-image-segmentation)
- [3D Medical Image Analysis](#3d-medical-image-analysis)
- [Text-Based Medical Language Models](#text-based-medical-language-models)
- [Radiology Report Generation](#radiology-report-generation)
- [Knowledge Distillation & Parameter-Efficient Fine-Tuning](#knowledge-distillation--parameter-efficient-fine-tuning)
- [Lumbar Spine Specialized Systems](#lumbar-spine-specialized-systems)
- [Object Detection Architectures](#object-detection-architectures)
- [Datasets & Benchmarks](#datasets--benchmarks)
- [Clinical AI Deployment & Validation](#clinical-ai-deployment--validation)
- [Statistical & Evaluation Methods](#statistical--evaluation-methods)

---

# Survey & Review Papers

**Deep Learning in Neural Networks: An Overview.** [2015].<br>
*J. Schmidhuber.*<br>
Neural Networks, vol. 61, pp. 85–117.<br>
[[PDF](https://doi.org/10.1016/j.neunet.2014.09.003)]

**A Survey on Deep Learning in Medical Image Analysis.** [2017].<br>
*G. Litjens, T. Kooi, B. E. Bejnordi, A. A. A. Setio, F. Ciompi, M. Ghafoorian, J. A. W. M. van der Laak, B. van Ginneken, C. I. Sánchez.*<br>
Medical Image Analysis, vol. 42, pp. 60–88.<br>
[[PDF](https://doi.org/10.1016/j.media.2017.07.005)]

**A Review: Deep Learning for Medical Image Segmentation Using Multi-Modality Fusion.** [2019].<br>
*T. Zhou, S. Ruan, S. Canu.*<br>
Array, vol. 3–4, pp. 100004.<br>
[[PDF](https://doi.org/10.1016/j.array.2019.100004)]

**Knowledge Distillation: A Survey.** [2021].<br>
*J. Gou, B. Yu, S. J. Maybank, D. Tao.*<br>
International Journal of Computer Vision, vol. 129(6), pp. 1789–1819.<br>
[[PDF](https://doi.org/10.1007/s11263-021-01453-z)]

**Knowledge Distillation In Medical Data Mining: A Survey.** [Oct. 2021].<br>
*H. Meng, Z. Lin, F. Yang, Y. Xu, L. Cui.*<br>
5th International Conference on Crowd Science and Engineering, pp. 175–182.<br>
[[PDF](https://doi.org/10.1145/3503181.3503211)]

**Transformers in Medical Imaging: A Survey.** [2023]. Medical Image Analysis.<br>
*F. Shamshad, S. Khan, S. W. Zamir, M. H. Khan, M. Hayat, F. S. Khan, H. Fu.*<br>
Medical Image Analysis, vol. 88, pp. 102802.<br>
[[PDF](https://doi.org/10.1016/j.media.2023.102802)]

**Computer-Vision Benchmark Segment-Anything Model (SAM) in Medical Images: Accuracy in 12 Datasets.** [2023].<br>
*S. He, R. Bao, J. Li, J. Stout, A. Bjornerud, P. E. Grant, Y. Ou.*<br>
arXiv:2304.09324.<br>
[[PDF](https://arxiv.org/abs/2304.09324)]

**Segment Anything Model for Medical Image Analysis: An Experimental Study.** [2023].<br>
*M. A. Mazurowski, H. Dong, H. Gu, J. Yang, N. Konz, Y. Zhang.*<br>
Medical Image Analysis, vol. 89, pp. 102918.<br>
[[PDF](https://doi.org/10.1016/j.media.2023.102918)]

**Survey of Hallucination in Natural Language Generation.** [2023].<br>
*Z. Ji, N. Lee, R. Frieske, T. Yu, D. Su, Y. Xu, E. Ishii, Y. J. Bang, A. Madotto, P. Fung.*<br>
ACM Computing Surveys, vol. 55(12), pp. 1–38.<br>
[[PDF](https://doi.org/10.1145/3571730)]

**A Survey of Large Language Models for Healthcare: From Data, Technology, and Applications to Accountability and Ethics.** [2023].<br>
*K. He et al.*<br>
arXiv:2310.05694.<br>
[[PDF](https://arxiv.org/abs/2310.05694)]

**A survey of large language models in medicine.** [2023].<br>
*W. Liao et al.*<br>
arXiv:2311.05112.<br>
[[PDF](https://arxiv.org/abs/2311.05112)]

**Generalist Vision Foundation Models for Medical Imaging: A Case Study of Segment Anything Model on Zero-Shot Medical Segmentation.** [2023].<br>
*P. Shi, J. Qiu, S. M. D. Aodeng, H. Wei, F. P.-W. Lo, W. Yuan.*<br>
Diagnostics, vol. 13(11), pp. 1947.<br>
[[PDF](https://doi.org/10.3390/diagnostics13111947)]

**A survey on medical large language models: Technology, application, trustworthiness, and future directions.** [2024].<br>
*L. Liu, X. Yang, J. Lei, Y. Shen, J. Wang, P. Wei, Z. Chu, Z. Qin, K. Ren.*<br>
arXiv:2406.03712.<br>
[[PDF](https://arxiv.org/abs/2406.03712)]

**A Survey on Model Compression for Large Language Models.** [2024].<br>
*X. Zhu, J. Li, Y. Liu, C. Ma, W. Wang.*<br>
arXiv:2308.07633.<br>
[[PDF](https://arxiv.org/abs/2308.07633)]

**A Survey on Knowledge Distillation of Large Language Models.** [2024].<br>
*Z. Xu et al.*<br>
arXiv:2402.13116.<br>
[[PDF](https://arxiv.org/abs/2402.13116)]

**Advances in medical image segmentation: A comprehensive survey with a focus on lumbar spine applications.** [2024].<br>
*R. Azad et al.*<br>
arXiv:2510.03318.<br>
[[PDF](https://arxiv.org/abs/2510.03318)]

**Deep Learning Assisted Segmentation of the Lumbar Intervertebral Disc: A Systematic Review and Meta-Analysis.** [2024].<br>
*A. Wang et al.*<br>
Journal of Orthopaedic Surgery and Research, vol. 19(1), pp. 496.<br>
[[PDF](https://doi.org/10.1186/s13018-024-05002-5)]

**Advances in medical image segmentation: A comprehensive survey with a focus on lumbar spine applications.** [2025].<br>
*A. Kabil, G. Khoriba, M. Yousef, E. A. Rashed.*<br>
Computers in Biology and Medicine, vol. 198, pp. 111171.<br>
[[PDF](https://doi.org/10.1016/j.compbiomed.2025.111171)]

**Vision-Language Models in Medical Image Analysis: From Simple Fusion to General Large Models.** [2025].<br>
*X. Li et al.*<br>
Information Fusion, vol. 118, pp. 102995.<br>
[[PDF](https://doi.org/10.1016/j.inffus.2025.102995)]

**Towards Comprehensive Benchmarking of Medical Vision Language Models.** [2025].<br>
*D. Khatri, S. T. P. Gupta.*<br>
Briefings in Bioinformatics, vol. 26(Suppl 1), pp. i24–i25.<br>
[[PDF](https://doi.org/10.1093/bib/bbaf631.035)]

**Can We Trust AI Doctors? A Survey of Medical Hallucination in Large Language and Large Vision-Language Models.** [2025].<br>
*Z. Zhu, Y. Zhang, X. Zhuang, F. Zhang, Z. Wan, Y. Chen, Q. Long, Y. Zheng, X. Wu.*<br>
Findings of the Association for Computational Linguistics: ACL 2025, pp. 6748–6769.<br>
[[PDF](https://doi.org/10.18653/v1/2025.findings-acl.350)]

**Medical Large Language Models and Systems in the Clinical Application of Spinal Diseases: Current Status, Challenges, and Future Prospects.** [2026].<br>
*W. Tang, R. Chen, X. Long, D. Yu, S. Zhao, B. Chen.*<br>
Journal of Orthopaedic Translation, vol. 57, pp. 101050.<br>
[[PDF](https://doi.org/10.1016/j.jot.2026.101050)]

**A systematic review of vision language models: Comprehensive analysis of architectures, applications, datasets and challenges towards robust multimodal intelligence.** [2026].<br>
*A. Rahman.*<br>
Array, pp. 100739.<br>
[[PDF](https://doi.org/10.1016/j.array.2026.100739)]

**Clinical AI in Radiology: Foundations, Trends, Applications, and Emerging Directions.** [2026].<br>
*I. Hartsock, N. Koutsoubis, S. Ahmed, N. Parker, M. B. Schabath, C. Araujo, A. Qayyum, C. Lam, R. A. Gatenby, G. Rasool.*<br>
Cancers, vol. 18(6), pp. 942.<br>
[[PDF](https://doi.org/10.3390/cancers18060942)]

---

# Foundational Architectures & Deep Learning

**Deep Learning.** [2015].<br>
*Y. LeCun, Y. Bengio, G. Hinton.*<br>
Nature, vol. 521(7553), pp. 436–444.<br>
[[PDF](https://doi.org/10.1038/nature14539)]

**Fully Convolutional Networks for Semantic Segmentation.** [2015] [CVPR].<br>
*J. Long, E. Shelhamer, T. Darrell.*<br>
[[PDF](https://doi.org/10.1109/CVPR.2015.7298965)]

**Deep Residual Learning for Image Recognition.** [2016] [CVPR].<br>
*K. He, X. Zhang, S. Ren, J. Sun.*<br>
[[PDF](https://doi.org/10.1109/CVPR.2016.90)]

**Attention is All You Need.** [2017] [NeurIPS].<br>
*A. Vaswani, N. Shazeer, N. Parmar, J. Uszkoreit, L. Jones, A. N. Gomez, Ł. Kaiser, I. Polosukhin.*<br>
Advances in Neural Information Processing Systems, vol. 30, pp. 5998–6008.<br>
[[PDF](https://proceedings.neurips.cc/paper/2017/hash/3f5ee243547dee91fbd053c1c4a845aa-Abstract.html)]

**Densely Connected Convolutional Networks.** [2017] [CVPR].<br>
*G. Huang, Z. Liu, L. van der Maaten, K. Q. Weinberger.*<br>
[[PDF](https://doi.org/10.1109/CVPR.2017.243)]

**Dermatologist-level classification of skin cancer with deep neural networks.** [2017].<br>
*A. Esteva, B. Kuprel, R. A. Novoa, J. Ko, S. M. Swetter, H. M. Blau, S. Thrun.*<br>
Nature, vol. 542(7639), pp. 115–118.<br>
[[PDF](https://doi.org/10.1038/nature21056)]

**BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding.** [2019] [NAACL-HLT].<br>
*J. Devlin, M.-W. Chang, K. Lee, K. Toutanova.*<br>
[[PDF](https://doi.org/10.18653/v1/N19-1423)]

**EfficientNet: Rethinking Model Scaling for Convolutional Neural Networks.** [2019] [ICML].<br>
*M. Tan, Q. V. Le.*<br>
[[PDF](https://arxiv.org/abs/1905.11946)]

**Language Models are Unsupervised Multitask Learners.** [2019].<br>
*A. Radford, J. Wu, R. Child, D. Luan, D. Amodei, I. Sutskever.*<br>
OpenAI Blog.<br>
[[PDF](https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf)]

**Language Models are Few-Shot Learners.** [2020] [NeurIPS].<br>
*T. Brown, B. Mann, N. Ryder, M. Subbiah, J. D. Kaplan, P. Dhariwal, A. Neelakantan et al.*<br>
Advances in Neural Information Processing Systems, vol. 33, pp. 1877–1901.<br>
[[PDF](https://proceedings.neurips.cc/paper/2020/hash/1457c0d6bfcb4967418bfb8ac142f64a-Abstract.html)]

**Generative Adversarial Networks.** [2020].<br>
*I. Goodfellow, J. Pouget-Abadie, M. Mirza, B. Xu, D. Warde-Farley, S. Ozair, A. Courville, Y. Bengio.*<br>
Communications of the ACM, vol. 63(11), pp. 139–144.<br>
[[PDF](https://doi.org/10.1145/3422622)]

**Transformers: State-of-the-Art Natural Language Processing.** [2020] [EMNLP Demos].<br>
*T. Wolf et al.*<br>
[[PDF](https://doi.org/10.18653/v1/2020.emnlp-demos.6)]

**An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale.** [2021] [ICLR].<br>
*A. Dosovitskiy, L. Beyer, A. Kolesnikov, D. Weissenborn, X. Zhai, T. Unterthiner, M. Dehghani, M. Minderer, G. Heigold, S. Gelly, J. Uszkoreit, N. Houlsby.*<br>
[[PDF](https://arxiv.org/abs/2010.11929)]

**Learning Transferable Visual Models From Natural Language Supervision.** [2021] [ICML].<br>
*A. Radford, J. W. Kim, C. Hallacy, A. Ramesh, G. Goh, S. Agarwal, G. Sastry, A. Askell, P. Mishkin, J. Clark, G. Krueger, I. Sutskever.*<br>
[[PDF](https://arxiv.org/abs/2103.00020)]

**Swin Transformer: Hierarchical Vision Transformer Using Shifted Windows.** [2021] [ICCV].<br>
*Z. Liu, Y. Lin, Y. Cao, H. Hu, Y. Wei, Z. Zhang, S. Lin, B. Guo.*<br>
[[PDF](https://doi.org/10.1109/ICCV48922.2021.00986)]

**DINOv2: Learning Robust Visual Features without Supervision.** [2023].<br>
*M. Oquab, T. Darcet, T. Moutakanni, H. V. Vo, M. Szafraniec, V. Khalidov, P. Fernandez et al.*<br>
Transactions on Machine Learning Research (TMLR), 2024.<br>
[[PDF](https://arxiv.org/abs/2304.07193)]

**SigLIP: Sigmoid loss for language image pre-training.** [2023] [ICCV].<br>
*X. Zhai, B. Mustafa, A. Kolesnikov, L. Beyer.*<br>
[[PDF](https://doi.org/10.48550/arXiv.2303.15343)]

---

# General-Purpose Foundation Models

**Segment Anything.** [2023] [ICCV].<br>
*A. Kirillov, E. Mintun, N. Ravi, H. Mao, C. Rolland, L. Gustafson, T. Xiao, S. Whitehead, A. C. Berg, W.-Y. Lo, P. Dollár, R. Girshick.*<br>
[[PDF](https://doi.org/10.1109/ICCV51070.2023.00371)]

**LLaMA: Open and Efficient Foundation Language Models.** [2023].<br>
*H. Touvron, T. Lavril, G. Izacard, X. Martinet, M.-A. Lachaux, T. Lacroix, B. Rozière et al.*<br>
arXiv:2302.13971.<br>
[[PDF](https://arxiv.org/abs/2302.13971)]

**LLaMA 2: Open Foundation and Fine-Tuned Chat Models.** [2023].<br>
*H. Touvron, L. Martin, K. Stone, P. Albert, A. Almahairi, Y. Babaei et al.*<br>
arXiv:2307.09288.<br>
[[PDF](https://arxiv.org/abs/2307.09288)]

**Visual Instruction Tuning.** [2023] [NeurIPS].<br>
*H. Liu, C. Li, Q. Wu, Y. J. Lee.*<br>
[[PDF](https://arxiv.org/abs/2304.08485)]

**PaLM: Scaling Language Modeling with Pathways.** [2023].<br>
*A. Chowdhery, S. Narang, J. Devlin, M. Bosma, G. Mishra, A. Roberts et al.*<br>
Journal of Machine Learning Research, vol. 24(240), pp. 1–113.<br>
[[PDF](https://arxiv.org/abs/2204.02311)]

**Gemini: A Family of Highly Capable Multimodal Models.** [2023].<br>
*Gemini Team, R. Anil, S. Borgeaud, Y. Wu, J.-B. Alayrac, J. Yu et al.*<br>
arXiv:2312.11805.<br>
[[PDF](https://arxiv.org/abs/2312.11805)]

**BLIP-2: Bootstrapping Language-Image Pre-training with Frozen Image Encoders and Large Language Models.** [2023] [ICML].<br>
*J. Li, D. Li, S. Savarese, S. Hoi.*<br>
[[PDF](https://arxiv.org/abs/2301.12597)]

**InstructBLIP: Towards General-purpose Vision-Language Models with Instruction Tuning.** [2023] [NeurIPS].<br>
*W. Dai, J. Li, D. Li, A. M. H. Tiong, J. Zhao, W. Wang, B. Li, P. Fung, S. Hoi.*<br>
[[PDF](https://arxiv.org/abs/2305.06500)]

**Gemma: Open Models Based on Gemini Research and Technology.** [2024].<br>
*Gemma Team, T. Mesnard, C. Hardin, R. Dadashi, S. Bhupatiraju et al.*<br>
arXiv:2403.08295.<br>
[[PDF](https://arxiv.org/abs/2403.08295)]

**MiniGPT-4: Enhancing Vision-Language Understanding with Advanced Large Language Models.** [2024] [ICLR].<br>
*D. Zhu, J. Chen, X. Shen, X. Li, M. Elhoseiny.*<br>
[[PDF](https://arxiv.org/abs/2304.10592)]

**Improved Baselines with Visual Instruction Tuning.** [2024] [CVPR].<br>
*H. Liu, C. Li, Y. Li, Y. J. Lee.*<br>
[[PDF](https://arxiv.org/abs/2310.03744)]

**InternVL: Scaling up Vision Foundation Models and Aligning for Generic Visual-Linguistic Tasks.** [2024] [CVPR].<br>
*Z. Chen, J. Wu, W. Wang et al.*<br>
[[PDF](https://doi.org/10.1109/CVPR52733.2024.02283)]

**Gemini 1.5: Unlocking Multimodal Understanding Across Millions of Tokens of Context.** [2024].<br>
*Gemini Team, M. Reid, N. Savinov, D. Teplyashin et al.*<br>
arXiv:2403.05530.<br>
[[PDF](https://arxiv.org/abs/2403.05530)]

**SAM 2: Segment Anything in Images and Videos.** [2024].<br>
*N. Ravi, V. Gabeur, Y.-T. Hu, R. Hu, C. Ryali, T. Ma, H. Khedr et al.*<br>
arXiv:2408.00714.<br>
[[PDF](https://arxiv.org/abs/2408.00714)]

**Gemma 3 Technical Report.** [2025].<br>
*Gemma Team.*<br>
arXiv:2503.19786.<br>
[[PDF](https://arxiv.org/abs/2503.19786)]

**Gemma 4 Model Card.** [2026].<br>
*Gemma Team, Google DeepMind.*<br>
Released 31 March 2026. Apache 2.0 licence.<br>
[[Link](https://ai.google.dev/gemma/docs/core/model_card_4)]

---

# Medical Vision-Language Models

**MedCLIP: Contrastive Learning from Unpaired Medical Images and Text.** [2022] [EMNLP].<br>
*Z. Wang, Z. Wu, D. Agarwal, J. Sun.*<br>
[[PDF](https://doi.org/10.18653/v1/2022.emnlp-main.256)]

**Foundation models for generalist medical artificial intelligence.** [2023].<br>
*M. Moor, O. Banerjee, Z. S. H. Abad, H. M. Krumholz, J. Leskovec, E. J. Topol, P. Rajpurkar.*<br>
Nature, vol. 616(7956), pp. 259–265.<br>
[[PDF](https://doi.org/10.1038/s41586-023-05881-4)]

**Large language models encode clinical knowledge.** [2023].<br>
*K. Singhal, S. Azizi, T. Tu, S. S. Mahdavi, J. Wei, H. W. Chung et al.*<br>
Nature, vol. 620(7972), pp. 172–180.<br>
[[PDF](https://doi.org/10.1038/s41586-023-06291-2)]

**Large language models in medicine.** [2023].<br>
*A. J. Thirunavukarasu, D. S. J. Ting, K. Elangovan, L. Gutierrez, T. F. Tan, D. S. W. Ting.*<br>
Nature Medicine, vol. 29(8), pp. 1930–1940.<br>
[[PDF](https://doi.org/10.1038/s41591-023-02448-8)]

**Capabilities of GPT-4 on Medical Challenge Problems.** [2023].<br>
*H. Nori, N. King, S. M. McKinney, D. Carignan, E. Horvitz.*<br>
arXiv:2303.13375.<br>
[[PDF](https://arxiv.org/abs/2303.13375)]

**GPT-4 Technical Report.** [2023].<br>
*OpenAI.*<br>
arXiv:2303.08774.<br>
[[PDF](https://arxiv.org/abs/2303.08774)]

**LLaVA-Med: Training a Large Language-and-Vision Assistant for Biomedicine in One Day.** [2023] [NeurIPS].<br>
*C. Li, C. Wong, S. Zhang, N. Usuyama, H. Liu, J. Yang, T. Naumann, H. Poon, J. Gao.*<br>
[[PDF](https://arxiv.org/abs/2306.00890)]

**Med-Flamingo: A Multimodal Medical Few-Shot Learner.** [2023] [ML4H, NeurIPS Workshop].<br>
*M. Moor, Q. Huang, S. Wu, M. Yasunaga, C. Zakka, Y. Dalmia, E. P. Reis, P. Rajpurkar, J. Leskovec.*<br>
[[PDF](https://arxiv.org/abs/2307.15189)]

**BiomedCLIP: A Multimodal Biomedical Foundation Model Pretrained from Fifteen Million Scientific Image-Text Pairs.** [2023] [NeurIPS Datasets and Benchmarks Track].<br>
*S. Zhang, Y. Xu, N. Usuyama, H. Xu, J. Bagga, R. Tinn, S. Preston, R. Rao, M. Wei, N. Valluri, C. Wong, T. Naumann, H. Poon.*<br>
[[PDF](https://arxiv.org/abs/2303.00915)]

**PMC-LLaMA: Towards Building Open-source Language Models for Medicine.** [2023].<br>
*C. Wu, W. Lin, X. Zhang, Y. Zhang, Y. Wang, W. Xie.*<br>
arXiv:2304.14454.<br>
[[PDF](https://arxiv.org/abs/2304.14454)]

**Towards Generalist Foundation Model for Radiology by Leveraging Web-Scale 2D & 3D Medical Data.** [2023].<br>
*C. Wu, X. Zhang, Y. Zhang, Y. Wang, W. Xie.*<br>
arXiv:2308.02463.<br>
[[PDF](https://arxiv.org/abs/2308.02463)]

**XrayGPT: Chest Radiographs Summarization using Medical Vision-Language Models.** [2023].<br>
*O. Thawkar, A. Shaker, S. P. Mullappilly, H. Cholakkal, R. M. Anwer, S. Khan, J. Laaksonen, F. S. Khan.*<br>
arXiv:2306.07971.<br>
[[PDF](https://arxiv.org/abs/2306.07971)]

**MAIRA-1: A Specialised Large Multimodal Model for Radiology Report Generation.** [2023].<br>
*S. L. Hyland, S. Bannur et al.*<br>
arXiv:2311.13668.<br>
[[PDF](https://arxiv.org/abs/2311.13668)]

**Visual Med-Alpaca: A Parameter-Efficient Biomedical LLM with Visual Capabilities.** [2023].<br>
*C. Shu, B. Chen, F. Liu, Z. Fu, E. Shareghi, N. Collier.*<br>
Language Technology Lab, University of Cambridge.<br>
[[Github](https://github.com/cambridgeltl/visual-med-alpaca)]

**Learning to Exploit Temporal Structure for Biomedical Vision-Language Processing.** [2023] [CVPR].<br>
*S. Bannur, S. Hyland, Q. Liu, F. Perez-Garcia, M. Ilse, D. C. Castro et al.*<br>
[[PDF](https://doi.org/10.1109/CVPR52729.2023.01442)]

**DoctorGLM: Fine-Tuning your Chinese Doctor is not a Herculean Task.** [2023].<br>
*H. Xiong, S. Wang, Y. Zhu, Z. Zhao, Y. Liu, Q. Wang, D. Shen.*<br>
arXiv:2304.01097.<br>
[[PDF](https://arxiv.org/abs/2304.01097)]

**Towards Generalist Biomedical AI.** [2024].<br>
*T. Tu, S. Azizi, D. Driess, M. Schaekermann, M. Amin, P.-H. Chang et al.*<br>
NEJM AI, vol. 1(3).<br>
[[PDF](https://doi.org/10.1056/AIoa2300138)]

**CheXagent: Towards a Foundation Model for Chest X-Ray Interpretation.** [2024].<br>
*Z. Chen, J. M. Varma, D. Wan, R. G. Barber et al.*<br>
arXiv:2401.12208.<br>
[[PDF](https://arxiv.org/abs/2401.12208)]

**MAIRA-2: Grounded Radiology Report Generation.** [2024].<br>
*S. Bannur, S. Hyland, Q. Liu, F. Pérez-García et al.*<br>
arXiv:2406.04449.<br>
[[PDF](https://arxiv.org/abs/2406.04449)]

**STLLaVA-Med: Self-training large language and vision assistant for medical question-answering.** [2024].<br>
*G. Sun et al.*<br>
arXiv:2406.19973.<br>
[[PDF](https://arxiv.org/abs/2406.19973)]

**Mitigating Hallucination in Large Multi-Modal Models via Robust Instruction Tuning.** [2024] [ICLR].<br>
*F. Liu et al.*<br>
[[PDF](https://arxiv.org/abs/2306.14565)]

**PMC-VQA: Visual Instruction Tuning for Medical Visual Question Answering.** [2024].<br>
*X. Zhang et al.*<br>
arXiv:2305.10415.<br>
[[PDF](https://arxiv.org/abs/2305.10415)]

**Towards building multilingual language model for medicine.** [2024].<br>
*P. Qiu, C. Wu, X. Zhang, W. Lin, H. Wang, Y. Zhang, Y. Wang, W. Xie.*<br>
Nature Communications, vol. 15(1), pp. 8384.<br>
[[PDF](https://doi.org/10.1038/s41467-024-52417-z)]

**Capabilities of Gemini Models in Medicine.** [2024].<br>
*K. Saab, T. Tu, W.-H. Weng, R. Tanno, D. Stutz et al.*<br>
arXiv:2404.18416.<br>
[[PDF](https://arxiv.org/abs/2404.18416)]

**RULE: Reliable Multimodal RAG for Factuality in Medical Vision Language Models.** [2024].<br>
*P. Xia, K. Zhu, H. Li, H. Zhu, Y. Li, G. Li, L. Zhang, H. Yao.*<br>
arXiv:2407.05131.<br>
[[PDF](https://arxiv.org/abs/2407.05131)]

**MedCoT: Medical Chain of Thought via Hierarchical Expert.** [2024] [EMNLP].<br>
*J. Liu, Y. Wang, J. Du, J. T. Zhou, Z. Liu.*<br>
[[PDF](https://aclanthology.org/2024.emnlp-main.962/)]

**MedGemma Technical Report.** [2025].<br>
*A. Sellergren et al.*<br>
arXiv:2507.05201.<br>
[[PDF](https://arxiv.org/abs/2507.05201)]

**A generalist medical language model for disease diagnosis assistance.** [2025].<br>
*X. Liu, H. Liu, G. Yang, Z. Jiang, S. Cui, Z. Zhang, H. Wang et al.*<br>
Nature Medicine, vol. 31(3), pp. 932–942.<br>
[[PDF](https://doi.org/10.1038/s41591-024-03416-6)]

**MedVisionLlama: Leveraging Pre-Trained Large Language Model Layers to Enhance Medical Image Segmentation.** [2025].<br>
*G. Marthi Krishna Kumar, A. Chadha, J. Mendola, A. Shmuel.*<br>
arXiv:2410.02458. Accepted at CVAMD Workshop, ICCVW 2025.<br>
[[PDF](https://arxiv.org/abs/2410.02458)]

**LLaVA-NeXT-Med: Medical Multimodal Large Language Model.** [2025] [CITSC].<br>
*Y. Guo, W. Huang.*<br>
[[PDF](https://doi.org/10.1109/CITSC64390.2025.00092)]

**Toward Expert-Level Medical Question Answering with Large Language Models.** [2025].<br>
*K. Singhal, T. Tu, J. Gottweis et al.*<br>
Nature Medicine, vol. 31, pp. 943–950.<br>
[[PDF](https://doi.org/10.1038/s41591-024-03423-7)]

**MedGemma 1.5 Technical Report.** [2026].<br>
*A. Sellergren, C. Gao, F. Mahvar, T. Kohlberger, F. Jamil et al.*<br>
arXiv:2604.05081.<br>
[[PDF](https://arxiv.org/abs/2604.05081)]

---

# Medical Image Segmentation

**U-Net: Convolutional Networks for Biomedical Image Segmentation.** [2015] [MICCAI].<br>
*O. Ronneberger, P. Fischer, T. Brox.*<br>
LNCS vol. 9351, pp. 234–241.<br>
[[PDF](https://doi.org/10.1007/978-3-319-24574-4_28)]

**V-Net: Fully Convolutional Neural Networks for Volumetric Medical Image Segmentation.** [2016] [3DV].<br>
*F. Milletari, N. Navab, S.-A. Ahmadi.*<br>
[[PDF](https://doi.org/10.1109/3DV.2016.79)]

**3D U-Net: Learning Dense Volumetric Segmentation from Sparse Annotation.** [2016] [MICCAI].<br>
*Ö. Çiçek, A. Abdulkadir, S. S. Lienkamp, T. Brox, O. Ronneberger.*<br>
LNCS vol. 9901, pp. 424–432.<br>
[[PDF](https://doi.org/10.1007/978-3-319-46723-8_49)]

**Generalised Dice Overlap as a Deep Learning Loss Function for Highly Unbalanced Segmentations.** [2017].<br>
*C. H. Sudre, W. Li, T. Vercauteren, S. Ourselin, M. J. Cardoso.*<br>
LNCS vol. 10553, pp. 240–248.<br>
[[PDF](https://doi.org/10.1007/978-3-319-67558-9_28)]

**3D MRI Brain Tumor Segmentation Using Autoencoder Regularization.** [2019] [MICCAI BrainLes Workshop].<br>
*A. Myronenko.*<br>
LNCS vol. 11384, pp. 311–320.<br>
[[PDF](https://doi.org/10.1007/978-3-030-11726-9_28)]

**UNet++: Redesigning Skip Connections to Exploit Multiscale Features in Image Segmentation.** [2020].<br>
*Z. Zhou, M. M. R. Siddiquee, N. Tajbakhsh, J. Liang.*<br>
IEEE Transactions on Medical Imaging, vol. 39(6), pp. 1856–1867.<br>
[[PDF](https://doi.org/10.1109/TMI.2019.2959609)]

**nnU-Net: A Self-Configuring Method for Deep Learning-Based Biomedical Image Segmentation.** [2021].<br>
*F. Isensee, P. F. Jaeger, S. A. A. Kohl, J. Petersen, K. H. Maier-Hein.*<br>
Nature Methods, vol. 18(2), pp. 203–211.<br>
[[PDF](https://doi.org/10.1038/s41592-020-01008-z)]

**TransUNet: Rethinking the U-Net Architecture Design for Medical Image Segmentation through the Lens of Transformers.** [2024].<br>
*J. Chen, Y. Lu, Q. Yu, X. Luo, E. Adeli, Y. Wang, L. Lu, A. L. Yuille, Y. Zhou.*<br>
Medical Image Analysis, vol. 97, pp. 103280.<br>
[[PDF](https://doi.org/10.1016/j.media.2024.103280)]

**Efficient Medical Image Segmentation Based on Knowledge Distillation.** [2021].<br>
*D. Qin, J.-J. Bu, Z. Liu, X. Shen, S. Zhou, J.-J. Gu, Z.-H. Wang, L. Wu, H.-F. Dai.*<br>
IEEE Transactions on Medical Imaging, vol. 40(12), pp. 3820–3831.<br>
[[PDF](https://doi.org/10.1109/TMI.2021.3098703)]

**MONAI: An open-source framework for deep learning in healthcare.** [2022].<br>
*M. J. Cardoso, W. Li, R. Brown, N. Ma, E. Kerfoot et al.*<br>
arXiv:2211.02701.<br>
[[PDF](https://arxiv.org/abs/2211.02701)]

**Self-Supervised Pre-Training of Swin Transformers for 3D Medical Image Analysis.** [2022] [CVPR].<br>
*Y. Tang, D. Yang, W. Li, H. R. Roth, B. Landman, D. Xu, V. Nath, A. Hatamizadeh.*<br>
[[PDF](https://doi.org/10.1109/CVPR52688.2022.02007)]

**Swin UNETR: Swin Transformers for Semantic Segmentation of Brain Tumors in MRI Images.** [2022] [MICCAI BrainLes Workshop].<br>
*A. Hatamizadeh, V. Nath, Y. Tang, D. Yang, H. R. Roth, D. Xu.*<br>
LNCS vol. 12962, pp. 272–284.<br>
[[PDF](https://doi.org/10.1007/978-3-031-08999-2_22)]

**CLIP-Driven Universal Model for Organ Segmentation and Tumor Detection.** [2023] [ICCV].<br>
*J. Liu et al.*<br>
[[PDF](https://doi.org/10.1109/ICCV51070.2023.01934)]

**UniverSeg: Universal Medical Image Segmentation.** [2023] [ICCV].<br>
*V. I. Butoi, J. J. Ortiz, T. Ma, M. R. Sabuncu, J. Guttag, A. V. Dalca.*<br>
[[PDF](https://arxiv.org/abs/2304.06131)]

**Segment anything in medical images.** [2024].<br>
*J. Ma, Y. He, F. Li, L. Han, C. You, B. Wang.*<br>
Nature Communications, vol. 15(1), pp. 654.<br>
[[PDF](https://doi.org/10.1038/s41467-024-44824-z)]

**SAM-Med3D: Towards General-Purpose Segmentation Models for Volumetric Medical Images.** [2024].<br>
*H. Wang, S. Guo, J. Ye, Z. Deng, J. Cheng, T. Li et al.*<br>
arXiv:2310.15161.<br>
[[PDF](https://arxiv.org/abs/2310.15161)]

**SAM-Med2D: Segment Anything in Medical 2D Images.** [2024].<br>
*J. Cheng, J. Ye, Z. Deng, J. Chen, T. Li, H. Wang et al.*<br>
arXiv:2308.16184.<br>
[[PDF](https://arxiv.org/abs/2308.16184)]

**MedCLIP-SAM: Bridging Text and Image Towards Universal Medical Image Segmentation.** [2024] [MICCAI].<br>
*T. Koleilat, H. Asgariandehkordi, H. Rivaz, Y. Xiao.*<br>
[[PDF](https://arxiv.org/abs/2403.20253)]

**MA-SAM: Modality-Agnostic SAM Adaptation for 3D Medical Image Segmentation.** [2024].<br>
*J. Chen et al.*<br>
Medical Image Analysis, vol. 98, pp. 103310.<br>
[[PDF](https://doi.org/10.1016/j.media.2024.103310)]

**SA-Med2D-20M: Segment Anything in Medical 2D Images with 20 Million Masks.** [2024].<br>
*J. Ye et al.*<br>
arXiv:2311.11969.<br>
[[PDF](https://arxiv.org/abs/2311.11969)]

**MedSAM-2: Segment Medical Images As Video Via Segment Anything Model 2.** [2025].<br>
*J. Zhu, A. Hamdi, Y. Qi, Y. Jin, J. Wu.*<br>
arXiv:2408.00874. Accepted at MICCAI 2025.<br>
[[PDF](https://arxiv.org/abs/2408.00874)]

**SAM2-Rad: A segmentation model for medical images with learnable prompts.** [2025].<br>
*A. S. Wahd, B. Felfeliyan, Y. Zhou, S. Ghosh, A. McArthur, J. Zhang, J. L. Jaremko, A. Hareendranathan.*<br>
Computers in Biology and Medicine, vol. 187, pp. 109725.<br>
[[PDF](https://doi.org/10.1016/j.compbiomed.2025.109725)]

**Self-prompt SAM: Medical image segmentation via automatic prompt SAM adaptation.** [2025].<br>
*B. Xie, H. Tang, D. Cai, Y. Yan, G. Agam.*<br>
arXiv:2502.00630.<br>
[[PDF](https://arxiv.org/abs/2502.00630)]

**MedSeg-R: Reasoning segmentation in medical images with multimodal large language models.** [2025].<br>
*Y. Huang, Z. Peng, Y. Zhao, P. Yang, X. Yang, W. Shen.*<br>
arXiv:2506.10465.<br>
[[PDF](https://arxiv.org/abs/2506.10465)]

**SAM-Med3D: A vision foundation model for general-purpose segmentation on volumetric medical images.** [2025].<br>
*H. Wang, S. Guo, J. Ye, Z. Deng, J. Cheng, T. Li et al.*<br>
IEEE Transactions on Neural Networks and Learning Systems.<br>
[[PDF](https://doi.org/10.1109/tnnls.2025.3586694)]

**Automated Lumbar Spine Segmentation in MRI Using an Enhanced U-Net with Inception Module and Dual-Output Mechanism.** [2025].<br>
*J. T. Silveira, G. S., P. P. Kundapur.*<br>
Scientific Reports, vol. 15(1), pp. 39215.<br>
[[PDF](https://doi.org/10.1038/s41598-025-20721-3)]

**Medical SAM3: A Foundation Model for Universal Prompt-Driven Medical Image Segmentation.** [2026].<br>
*C. Jiang, T. Ding, C. Song, J. Tu, Z. Yan, Y. Shao et al.*<br>
arXiv:2601.10880.<br>
[[PDF](https://arxiv.org/abs/2601.10880)]

---

# 3D Medical Image Analysis

**Developing generalist foundation models from a multimodal dataset for 3D computed tomography.** [2024].<br>
*I. E. Hamamci, S. Er, C. Wang, F. Almas, A. G. Simsek et al.*<br>
arXiv:2403.17834.<br>
[[PDF](https://arxiv.org/abs/2403.17834)]

**CT2Rep: Automated Radiology Report Generation for 3D Medical Imaging.** [2024].<br>
*I. E. Hamamci, S. Er, E. Alkan et al.*<br>
arXiv:2403.06801.<br>
[[PDF](https://arxiv.org/abs/2403.06801)]

**M3D: Advancing 3D Medical Image Analysis with Multi-Modal Large Language Models.** [2024].<br>
*F. Bai, Y. Du, T. Huang, M. Q.-H. Meng, B. Zhao.*<br>
arXiv:2404.00578.<br>
[[PDF](https://arxiv.org/abs/2404.00578)]

**Vision-language foundation model for 3D medical imaging.** [2025].<br>
*J. Wu, Y. Wang, Z. Zhong, W. Liao, N. Trayanova, Z. Jiao, H. X. Bai.*<br>
npj Artificial Intelligence, vol. 1(1), pp. 17.<br>
[[PDF](https://doi.org/10.1038/s44387-025-00015-9)]

**Med3DVLM: An Efficient Vision-Language Model for 3D Medical Image Analysis.** [2025].<br>
*Y. Xin, G. C. Ates, K. Gong, W. Shao.*<br>
IEEE Journal of Biomedical and Health Informatics (Early access).<br>
[[PDF](https://doi.org/10.1109/JBHI.2025.3604595)]

---

# Text-Based Medical Language Models

**Publicly Available Clinical BERT Embeddings.** [2019].<br>
*E. Alsentzer, J. R. Murphy, W. Boag, W.-H. Weng, D. Jin, T. Naumann, M. B. A. McDermott.*<br>
arXiv:1904.03323.<br>
[[PDF](https://arxiv.org/abs/1904.03323)]

**BioBERT: A pre-trained biomedical language representation model for biomedical text mining.** [2020].<br>
*J. Lee, W. Yoon, S. Kim, D. Kim, S. Kim, C. H. So, J. Kang.*<br>
Bioinformatics, vol. 36(4), pp. 1234–1240.<br>
[[PDF](https://doi.org/10.1093/bioinformatics/btz682)]

**Domain-Specific Language Model Pretraining for Biomedical Natural Language Processing.** [2022].<br>
*Y. Gu, R. Tinn, H. Cheng, M. Lucas, N. Usuyama, X. Liu, T. Naumann, J. Gao, H. Poon.*<br>
ACM Transactions on Computing for Healthcare, vol. 3(1), pp. 1–23.<br>
[[PDF](https://doi.org/10.1145/3458754)]

**BioGPT: Generative Pre-trained Transformer for Biomedical Text Generation and Mining.** [2022].<br>
*R. Luo, L. Sun, Y. Xia, T. Qin, S. Zhang, H. Poon, T.-Y. Liu.*<br>
Briefings in Bioinformatics, vol. 23(6), pp. bbac409.<br>
[[PDF](https://doi.org/10.1093/bib/bbac409)]

**GatorTron: A Large Clinical Language Model to Unlock Patient Information from Unstructured Electronic Health Records.** [2022].<br>
*X. Yang, A. Chen, P. G. Patel, H. Tran, D. Wu et al.*<br>
arXiv:2203.03540.<br>
[[PDF](https://arxiv.org/abs/2203.03540)]

**A Study of Generative Large Language Model for Medical Research and Healthcare.** [2023].<br>
*C. Peng, X. Yang, A. Chen, K. E. Smith, N. PourNejatian et al.*<br>
npj Digital Medicine, vol. 6(1), pp. 210.<br>
[[PDF](https://doi.org/10.1038/s41746-023-00958-w)]

**MEDITRON-70B: Scaling Medical Pretraining for Large Language Models.** [2023].<br>
*Z. Chen, A. H. Cano, A. Romanou, A. Bonnet, K. Matoba et al.*<br>
arXiv:2311.16079.<br>
[[PDF](https://arxiv.org/abs/2311.16079)]

**Med-Alpaca: An Open-Source Collection of Medical Conversational AI Models and Training Data.** [2023].<br>
*T. Z. Huang et al.*<br>
arXiv:2304.08247.<br>
[[PDF](https://arxiv.org/abs/2304.08247)]

**BioMedLM: A 2.7B Parameter Language Model Trained on Biomedical Text.** [2024].<br>
*E. Bolton, D. Hall, M. Yasunaga, T. Lee, C. Manning, P. Liang.*<br>
arXiv:2403.18421.<br>
[[PDF](https://arxiv.org/abs/2403.18421)]

---

# Radiology Report Generation

**RadLex: A New Method for Indexing Online Educational Materials.** [2006].<br>
*C. P. Langlotz.*<br>
RadioGraphics, vol. 26(6), pp. 1595–1597.<br>
[[PDF](https://doi.org/10.1148/rg.266065168)]

**On the Automatic Generation of Medical Imaging Reports.** [2018] [ACL].<br>
*B. Jing, P. Xie, E. Xing.*<br>
[[PDF](https://doi.org/10.18653/v1/P18-1240)]

**ESR Paper on Structured Reporting in Radiology.** [2018].<br>
*European Society of Radiology (ESR).*<br>
Insights into Imaging, vol. 9(1), pp. 1–7.<br>
[[PDF](https://doi.org/10.1007/s13244-017-0588-8)]

**Generating Radiology Reports via Memory-Driven Transformer.** [2020] [EMNLP].<br>
*Z. Chen, Y. Song, T.-H. Chang, X. Wan.*<br>
[[PDF](https://doi.org/10.18653/v1/2020.emnlp-main.112)]

**Structured Reporting in Radiology: A Systematic Review to Explore its Potential.** [2022].<br>
*J. M. Nobel, K. van Geel, S. G. F. Robben.*<br>
European Radiology, vol. 32, pp. 2837–2854.<br>
[[PDF](https://doi.org/10.1007/s00330-021-08327-5)]

**R2GenGPT: Radiology Report Generation with Frozen LLMs.** [2023].<br>
*Z. Wang et al.*<br>
Meta-Radiology, vol. 1(3), pp. 100033.<br>
[[PDF](https://doi.org/10.1016/j.metrad.2023.100033)]

**Interactive and Explainable Region-Guided Radiology Report Generation.** [2023] [CVPR].<br>
*T. Tanida, P. Müller, G. Kaissis, D. Rueckert.*<br>
[[PDF](https://doi.org/10.1109/CVPR52729.2023.00718)]

**RaDialog: A Large Vision-Language Model for Radiology Report Generation and Conversational Assistance.** [2023].<br>
*C. Pellegrini, M. Keicher, E. Özsoy, N. Navab.*<br>
arXiv:2311.18681.<br>
[[PDF](https://arxiv.org/abs/2311.18681)]

**Translating radiology reports into plain language using ChatGPT and GPT-4 with prompt learning.** [2023].<br>
*Q. Lyu, J. Tan, M. E. Zapadka, J. Ponnatapura, C. Niu, K. J. Myers, G. Wang, C. T. Whitlow.*<br>
Visual Computing for Industry, Biomedicine, and Art, vol. 6(1).<br>
[[PDF](https://doi.org/10.1186/s42492-023-00136-5)]

**Leveraging GPT-4 for Post Hoc Transformation of Free-Text Radiology Reports into Structured Reporting: A Multilingual Feasibility Study.** [2023].<br>
*L. C. Adams et al.*<br>
Radiology, vol. 307(4), pp. e230725.<br>
[[PDF](https://doi.org/10.1148/radiol.230725)]

**RSNA Radiology Reporting Templates.** [2024].<br>
*Radiological Society of North America (RSNA).*<br>
[[Link](https://radreport.org/)]

**CoMT: Chain-of-Medical-Thought Reduces Hallucination in Medical Report Generation.** [2024].<br>
*Y. Jiang, J. Chen, D. Yang, M. Li, S. Wang, T. Wu, K. Li, L. Zhang.*<br>
arXiv:2406.11451.<br>
[[PDF](https://arxiv.org/abs/2406.11451)]

**Direct Preference Optimization for Suppressing Hallucinated Prior Exams in Radiology Report Generation.** [2024].<br>
*O. Banerjee, H.-Y. Zhou, S. Adithan, S. Kwak, K. Wu, P. Rajpurkar.*<br>
arXiv:2406.06496.<br>
[[PDF](https://arxiv.org/abs/2406.06496)]

**The Application of Foundation Models in Radiology: Bridging Images, Reports, and Beyond.** [2025].<br>
*D. Lee.*<br>
Journal of the Korean Society of Radiology, vol. 86(6), pp. 919.<br>
[[PDF](https://doi.org/10.3348/jksr.2025.0048)]

**RADAR: A Multimodal Benchmark for 3D Image-Based Radiology Report Review.** [2026].<br>
*Z. Sun, M. Jagtiani, W. Yim, F. Xia, M. Gunn, M. Yetisgen, A. Ben Abacha.*<br>
arXiv:2603.06681.<br>
[[PDF](https://arxiv.org/abs/2603.06681)]

**Prospective evaluation of artificial intelligence (AI) in lumbar spine magnetic resonance imaging (MRI) workflow: from deep learning (DL)-enhanced accelerated acquisition to simultaneous vision-language model (VLM)-based automated report generation.** [2026].<br>
*J. Park, K. Han, J. S. Oh et al.*<br>
European Journal of Radiology, vol. 196, pp. 112695.<br>
[[PDF](https://doi.org/10.1016/j.ejrad.2026.112695)]

**Assessing the ability of large language models to simplify lumbar spine imaging reports into patient-facing text: a pilot study of GPT-4.** [2026].<br>
*R. Khazanchi, A. R. Chen, P. Desai, D. Herrera, J. R. Staub et al.*<br>
Skeletal Radiology, vol. 55(2), pp. 361–366.<br>
[[PDF](https://doi.org/10.1007/s00256-025-05027-9)]

---

# Knowledge Distillation & Parameter-Efficient Fine-Tuning

**Distilling the Knowledge in a Neural Network.** [2015].<br>
*G. Hinton, O. Vinyals, J. Dean.*<br>
arXiv:1503.02531.<br>
[[PDF](https://arxiv.org/abs/1503.02531)]

**FitNets: Hints for Thin Deep Nets.** [2015] [ICLR].<br>
*A. Romero, N. Ballas, S. E. Kahou, A. Chassang, C. Gatta, Y. Bengio.*<br>
[[PDF](https://arxiv.org/abs/1412.6550)]

**Paying More Attention to Attention: Improving the Performance of Convolutional Neural Networks via Attention Transfer.** [2017] [ICLR].<br>
*S. Zagoruyko, N. Komodakis.*<br>
[[PDF](https://arxiv.org/abs/1612.03928)]

**Parameter-Efficient Transfer Learning for NLP.** [2019] [ICML].<br>
*N. Houlsby, A. Girgis, S. Jastrzebski, B. Morrone, Q. de Laroussilhe, A. Gesmundo, M. Attariyan, S. Gelly.*<br>
[[PDF](https://arxiv.org/abs/1902.00751)]

**Relational Knowledge Distillation.** [2019] [CVPR].<br>
*W. Park, D. Kim, Y. Lu, M. Cho.*<br>
[[PDF](https://doi.org/10.1109/CVPR.2019.00409)]

**Contrastive Representation Distillation.** [2020] [ICLR].<br>
*Y. Tian, D. Krishnan, P. Isola.*<br>
[[PDF](https://arxiv.org/abs/1910.10699)]

**Embracing Imperfect Datasets: A Review of Deep Learning Solutions for Medical Image Segmentation.** [2020].<br>
*N. Tajbakhsh, L. Jeyaseelan, Q. Li, J. N. Chiang, Z. Wu, X. Ding.*<br>
Medical Image Analysis, vol. 63, pp. 101693.<br>
[[PDF](https://doi.org/10.1016/j.media.2020.101693)]

**The Power of Scale for Parameter-Efficient Prompt Tuning.** [2021] [EMNLP].<br>
*B. Lester, R. Al-Rfou, N. Constant.*<br>
[[PDF](https://doi.org/10.18653/v1/2021.emnlp-main.243)]

**LoRA: Low-Rank Adaptation of Large Language Models.** [2022] [ICLR].<br>
*E. J. Hu, Y. Shen, P. Wallis, Z. Allen-Zhu, Y. Li, S. Wang, L. Wang, W. Chen.*<br>
[[PDF](https://arxiv.org/abs/2106.09685)]

**Self-Supervised Learning in Medicine and Healthcare.** [2022].<br>
*R. Krishnan, P. Rajpurkar, E. J. Topol.*<br>
Nature Biomedical Engineering, vol. 6(12), pp. 1346–1352.<br>
[[PDF](https://doi.org/10.1038/s41551-022-00914-1)]

**Expert-Level Detection of Pathologies from Unannotated Chest X-Ray Images via Self-Supervised Learning.** [2022].<br>
*E. Tiu, E. Talius, P. Patel, C. P. Langlotz, A. Y. Ng, P. Rajpurkar.*<br>
Nature Biomedical Engineering, vol. 6(12), pp. 1399–1406.<br>
[[PDF](https://doi.org/10.1038/s41551-022-00936-9)]

**Knowledge distillation: A good teacher is patient and consistent.** [2022] [CVPR].<br>
*L. Beyer, X. Zhai, A. Royer, L. Markeeva, R. Anil, A. Kolesnikov.*<br>
[[PDF](https://doi.org/10.1109/CVPR52688.2022.01065)]

**LLaMA-Adapter: Efficient Fine-tuning of Language Models with Zero-init Attention.** [2023].<br>
*R. Zhang, J. Han, C. Liu, P. Gao, A. Zhou, X. Hu, S. Yan, P. Lu, H. Li, Y. Qiao.*<br>
arXiv:2303.16199.<br>
[[PDF](https://arxiv.org/abs/2303.16199)]

**TinyLLaVA: A Framework of Small-scale Large Multimodal Models.** [2024].<br>
*B. Zhou, Y. Hu, X. Weng, J. Jia, J. Luo, X. Liu, J. Wu, L. Huang.*<br>
arXiv:2402.14289.<br>
[[PDF](https://arxiv.org/abs/2402.14289)]

**VLM-KD: Knowledge Distillation from VLM for Long-Tail Visual Recognition.** [2024].<br>
*Z. Zhang, G. P. Meyer, Z. Lu, A. Shrivastava, A. Ravichandran, E. M. Wolff.*<br>
arXiv:2408.16930.<br>
[[PDF](https://arxiv.org/abs/2408.16930)]

**QLoRA: Efficient Finetuning of Quantized Language Models.** [2024] [NeurIPS].<br>
*T. Dettmers, A. Pagnoni, A. Holtzman, L. Zettlemoyer.*<br>
[[PDF](https://arxiv.org/abs/2305.14314)]

**Enhancing Medical Large Vision-Language Models via Alignment Distillation.** [2026] [AAAI].<br>
*A. Chang, T. Wang, F. Ma.*<br>
Proceedings of the AAAI Conference on Artificial Intelligence, vol. 40(24), pp. 19952–19960.<br>
[[PDF](https://doi.org/10.1609/aaai.v40i24.39079)]

---

# Lumbar Spine Specialized Systems

**Magnetic Resonance Classification of Lumbar Intervertebral Disc Degeneration.** [2001].<br>
*C. W. A. Pfirrmann, A. Metzdorf, M. Zanetti, J. Hodler, N. Boos.*<br>
Spine, vol. 26(17), pp. 1873–1878.<br>
[[PDF](https://doi.org/10.1097/00007632-200109010-00011)]

**Automated Radiological Grading of Spinal MRIs.** [2014].<br>
*M. Lootus, T. Kadir, A. Zisserman.*<br>
LNCS vol. 17, pp. 119–130.<br>
[[PDF](https://doi.org/10.1007/978-3-319-07269-2_10)]

**Detection and Labeling of Vertebrae in MR Images Using Deep Learning with Clinical Annotations as Training Data.** [2017].<br>
*D. Forsberg, E. Lundström, H. Ahlström et al.*<br>
Journal of Digital Imaging, vol. 30, pp. 406–412.<br>
[[PDF](https://doi.org/10.1007/s10278-017-9945-x)]

**SpineNet: Automated Classification and Evidence Visualization in Spinal MRIs.** [2017].<br>
*A. Jamaludin, T. Kadir, A. Zisserman.*<br>
Medical Image Analysis, vol. 41, pp. 63–73.<br>
[[PDF](https://doi.org/10.1016/j.media.2017.07.002)]

**Deep Spine: Automated Lumbar Vertebral Segmentation, Disc-Level Designation, and Spinal Stenosis Grading using Deep Learning.** [2018] [MLHC].<br>
*J.-T. Lu, S. Pedemonte, B. Bizzo, S. Doyle, K. P. Andriole, M. H. Michalski, R. G. Gonzalez, S. R. Pomerantz.*<br>
Proceedings of Machine Learning Research, vol. 85, pp. 403–419.<br>
[[PDF](https://proceedings.mlr.press/v85/lu18a.html)]

**Automated Pathogenesis-Based Diagnosis of Lumbar Neural Foraminal Stenosis via Deep Multiscale Multitask Learning.** [2018].<br>
*Z. Han, B. Wei, S. Leung et al.*<br>
Neuroinformatics, vol. 16(3–4), pp. 325–337.<br>
[[PDF](https://doi.org/10.1007/s12021-018-9365-1)]

**Iterative Fully Convolutional Neural Networks for Automatic Vertebra Segmentation and Identification.** [2019].<br>
*N. Lessmann, B. van Ginneken, P. A. de Jong, I. Išgum.*<br>
Medical Image Analysis, vol. 53, pp. 142–155.<br>
[[PDF](https://doi.org/10.1016/j.media.2019.02.005)]

**Automated Measurement of Lumbar Lordosis on Radiographs Using Machine Learning and Computer Vision.** [2020].<br>
*B. H. Cho, D. Kaji, Z. B. Cheung, I. B. Ye, R. Tang, A. Ahn, O. Carrillo, J. T. Schwartz, A. A. Valliani, E. K. Oermann, V. Arvind, D. Ranti, L. Sun, J. S. Kim, S. K. Cho.*<br>
Global Spine Journal, vol. 10(5), pp. 611–618.<br>
[[PDF](https://doi.org/10.1177/2192568219868190)]

**Deep Learning Model for Automated Detection and Classification of Central Canal, Lateral Recess, and Neural Foraminal Stenosis at Lumbar Spine MRI.** [2021].<br>
*J. T. P. D. Hallinan, L. Zhu, K. Yang, A. S. Makmur, A. Algazwi, Y. H. Lim et al.*<br>
Radiology, vol. 300(1), pp. 130–138.<br>
[[PDF](https://doi.org/10.1148/radiol.2021204289)]

**Deep learning-based vertebral body segmentation with extraction of spinal measurements and disorder disease classification.** [2022].<br>
*R. F. Masood, I. A. Taj, M. B. Khan, M. A. Qureshi, T. Hassan.*<br>
Biomedical Signal Processing and Control, vol. 74, pp. 103230.<br>
[[PDF](https://doi.org/10.1016/j.bspc.2021.103230)]

**Localization and Edge-Based Segmentation of Lumbar Spine Vertebrae to Identify the Deformities Using Deep Learning Models.** [2022].<br>
*M. Mushtaq, M. U. Akram, N. S. Alghamdi, J. Fatima, R. F. Masood.*<br>
Sensors, vol. 22(4), pp. 1547.<br>
[[PDF](https://doi.org/10.3390/s22041547)]

**A Composite Dataset of Lumbar Spine Images with Measurements and Disorders for AI-Based Medical Assistance.** [2022] [ICoDT2].<br>
*R. F. Masood, T. Hassan, H. Raja, B. Hassan, J. Dias, N. Werghi.*<br>
[[PDF](https://doi.org/10.1109/ICoDT255437.2022.9787452)]

**Using Natural Language Processing to Identify Low Back Pain in Imaging Reports.** [2022].<br>
*Y. Kim, C. Song, G. Song, S. B. Kim, H.-W. Han, I. Han.*<br>
Applied Sciences, vol. 12(24), pp. 12521.<br>
[[PDF](https://doi.org/10.3390/app122412521)]

**Automated Spinal MRI Labelling from Reports Using a Large Language Model.** [2024] [MICCAI].<br>
*R. Y. Park, R. Windsor, A. Jamaludin, A. Zisserman.*<br>
[[PDF](https://doi.org/10.1007/978-3-031-72086-4_10)]

**Classification of lumbar spine disorders using large language models and MRI segmentation.** [2024].<br>
*R. Dong, X. Cheng, M. Kang, Y. Qu.*<br>
BMC Medical Informatics and Decision Making, vol. 24(1), pp. 343.<br>
[[PDF](https://doi.org/10.1186/s12911-024-02740-8)]

**Lumbar spine segmentation in MR images: A dataset and a public benchmark.** [2024].<br>
*J. W. van der Graaf, M. L. van Hooff, C. F. M. Buckens, M. Rutten, J. L. C. van Susante, R. J. Kroeze, M. de Kleuver, B. van Ginneken, N. Lessmann.*<br>
Scientific Data, vol. 11(1), pp. 264.<br>
[[PDF](https://doi.org/10.1038/s41597-024-03098-5)]

**SpineFM: Leveraging Foundation Models for Automatic Spine X-ray Segmentation.** [2024].<br>
*S. J. Simons, B. W. Papież.*<br>
arXiv:2411.00326. Accepted at ISBI 2025.<br>
[[PDF](https://arxiv.org/abs/2411.00326)]

**Diffusion-Based Semantic Segmentation of Lumbar Spine MRI Scans of Lower Back Pain Patients.** [2024].<br>
*M. Monzon, T. Iff, E. Konukoglu, C. R. Jutzeler.*<br>
arXiv:2411.10755.<br>
[[PDF](https://arxiv.org/abs/2411.10755)]

**AutoSpineAI: Lightweight Multimodal CAD Framework for Lumbar Spine MRI Assessments.** [2025].<br>
*S. Salem, A. Habib, M. Raza, Z. Al-Huda, O. Al-maqtari, B. Ertuğrul, Ö. Yıldırım, Y. H. Gu, M. A. Al-antari.*<br>
[[PDF](https://openreview.net/pdf?id=RKOKlm4e4U)]

**AI-Driven MRI Spine Pathology Detection.** [2025].<br>
*B. Subramanian, N. Kumarasami, P. Shastry, R. Sripadraj, K. Sivasailam, D. Anandakumar, A. Ramachandran.*<br>
arXiv:2503.20316.<br>
[[PDF](https://arxiv.org/abs/2503.20316)]

**Automated Diagnosis and Grading of Lumbar Intervertebral Disc Degeneration Based on a Modified YOLO Framework.** [2025].<br>
*A. Wang, T. Wang, X. Liu, N. Fan, S. Yuan, P. Du, C. Zou, R. Chen, Y. Xi, Z. Gu, H. Song, Q. Fei, Y. Zhang, L. Zang.*<br>
Frontiers in Bioengineering and Biotechnology, vol. 13, pp. 1526478.<br>
[[PDF](https://doi.org/10.3389/fbioe.2025.1526478)]

**SpineBench: Benchmarking Multimodal LLMs for Spinal Pathology Analysis.** [2025] [ACM Multimedia].<br>
*C. Zhang, Z. Li, P. Li, X. Cui, S. Xia, W. Yan, Y. Zhang, Q. Zhuang.*<br>
[[PDF](https://doi.org/10.1145/3664647.3681580)]

**Deep Learning-Based Lumbar Spinal Canal Stenosis Classification Using MRI Scans.** [2025].<br>
*G. G. de Celis, W. Bukaita.*<br>
Medical Research Archives, vol. 13(7).<br>
[[PDF](https://doi.org/10.18103/mra.v13i7.6660)]

**Automated Lumbar Disc Intensity Classification From MRI Scans Using Region-Based CNNs and Transformer Models.** [2025].<br>
*H. Ulutas, M. F. Erkoc, E. Ozbay, M. E. Sahin, M. O. Karakus, E. Yuce.*<br>
International Journal of Imaging Systems and Technology, vol. 35(6), pp. e70229.<br>
[[PDF](https://doi.org/10.1002/ima.70229)]

**Deep Learning-Based Automated Segmentation and Quantification of the Dural Sac Cross-Sectional Area in Lumbar Spine MRI.** [2025].<br>
*G. Ghobrial, C. Roth.*<br>
Frontiers in Radiology, vol. 5, pp. 1503625.<br>
[[PDF](https://doi.org/10.3389/fradi.2025.1503625)]

---

# Object Detection Architectures

**Faster R-CNN: Towards Real-Time Object Detection with Region Proposal Networks.** [2015] [NeurIPS].<br>
*S. Ren, K. He, R. Girshick, J. Sun.*<br>
[[PDF](https://arxiv.org/abs/1506.01497)]

**You Only Look Once: Unified, Real-Time Object Detection.** [2016] [CVPR].<br>
*J. Redmon, S. Divvala, R. Girshick, A. Farhadi.*<br>
[[PDF](https://doi.org/10.1109/CVPR.2016.91)]

**End-to-End Object Detection with Transformers.** [2020] [ECCV].<br>
*N. Carion, F. Massa, G. Synnaeve, N. Usunier, A. Kirillov, S. Zagoruyko.*<br>
LNCS vol. 12346, pp. 213–229.<br>
[[PDF](https://doi.org/10.1007/978-3-030-58452-8_13)]

**Cascade R-CNN: Multi-Stage Object Detection.** [2021].<br>
*Z. Cai, N. Vasconcelos.*<br>
IEEE Transactions on Pattern Analysis and Machine Intelligence, vol. 43(5), pp. 1483–1498.<br>
[[PDF](https://doi.org/10.1109/TPAMI.2019.2956516)]

---

# Datasets & Benchmarks

**MIMIC-III, a Freely Accessible Critical Care Database.** [2016].<br>
*A. E. W. Johnson, T. J. Pollard, L. Shen, L.-w. H. Lehman, M. Feng, M. Ghassemi, B. Moody, P. Szolovits, L. A. Celi, R. G. Mark.*<br>
Scientific Data, vol. 3, pp. 160035.<br>
[[PDF](https://doi.org/10.1038/sdata.2016.35)]

**ChestX-ray8: Hospital-Scale Chest X-Ray Database and Benchmarks.** [2017] [CVPR].<br>
*X. Wang, Y. Peng, L. Lu, Z. Lu, M. Bagheri, R. M. Summers.*<br>
[[PDF](https://doi.org/10.1109/CVPR.2017.369)]

**CheXpert: A Large Chest Radiograph Dataset with Uncertainty Labels and Expert Comparison.** [2019] [AAAI].<br>
*J. Irvin, P. Rajpurkar, M. Ko, Y. Yu, S. Ciurea-Ilcus, C. Chute et al.*<br>
[[PDF](https://doi.org/10.1609/aaai.v33i01.3301590)]

**MIMIC-CXR, a De-identified Publicly Available Database of Chest Radiographs with Free-Text Reports.** [2019].<br>
*A. E. W. Johnson, T. J. Pollard, N. R. Greenbaum, M. P. Lungren, C.-y. Deng, Y. Peng, Z. Lu, R. G. Mark, S. J. Berkowitz, S. Horng.*<br>
Scientific Data, vol. 6(1), pp. 317.<br>
[[PDF](https://doi.org/10.1038/s41597-019-0322-0)]

**A Large Annotated Medical Image Dataset for the Development and Evaluation of Segmentation Algorithms.** [2019].<br>
*A. L. Simpson, M. Antonelli, S. Bakas, M. Bilello, K. Farahani, B. van Ginneken et al.*<br>
arXiv:1902.09063.<br>
[[PDF](https://arxiv.org/abs/1902.09063)]

**What Disease Does This Patient Have? A Large-Scale Open Domain Question Answering Dataset from Medical Exams.** [2021].<br>
*D. Jin, E. Pan, N. Oufattole, W.-H. Weng, H. Fang, P. Szolovits.*<br>
Applied Sciences, vol. 11(14), pp. 6421.<br>
[[PDF](https://doi.org/10.3390/app11146421)]

**VerSe: A Vertebrae Labelling and Segmentation Benchmark for Multi-Detector CT Images.** [2021].<br>
*A. Sekuboyina, M. E. Husseini, A. Bayat, M. Löffler, H. Liebl, H. Li, G. Tetteh et al.*<br>
Medical Image Analysis, vol. 73, pp. 102166.<br>
[[PDF](https://doi.org/10.1016/j.media.2021.102166)]

**MIMIC-IV, a Freely Accessible Electronic Health Record Dataset.** [2023].<br>
*A. Johnson, L. Bulgarelli, T. Pollard, S. Horng, L. A. Celi, R. Mark.*<br>
Scientific Data, vol. 10, pp. 1.<br>
[[PDF](https://doi.org/10.1038/s41597-022-01899-x)]

**The RSNA Lumbar Degenerative Imaging Spine Classification (LumbarDISC) Dataset.** [2026].<br>
*T. J. Richards, A. E. Flanders, E. Colak, L. M. Prevedello, R. L. Ball, F. Kitamura, J. Mongan et al.*<br>
Radiology: Artificial Intelligence, vol. 8(2).<br>
[[PDF](https://doi.org/10.1148/ryai.250480)]

---

# Clinical AI Deployment & Validation

**AI in Health and Medicine.** [2022].<br>
*P. Rajpurkar, E. Chen, O. Banerjee, E. J. Topol.*<br>
Nature Medicine, vol. 28(1), pp. 31–38.<br>
[[PDF](https://doi.org/10.1038/s41591-021-01614-0)]

**Multimodal Biomedical AI.** [2022].<br>
*J. N. Acosta, G. J. Falcone, P. Rajpurkar, E. J. Topol.*<br>
Nature Medicine, vol. 28(9), pp. 1773–1784.<br>
[[PDF](https://doi.org/10.1038/s41591-022-01981-2)]

**A Foundation Model for Generalizable Disease Detection from Retinal Images.** [2023].<br>
*Y. Zhou et al.*<br>
Nature, vol. 622, pp. 156–163.<br>
[[PDF](https://doi.org/10.1038/s41586-023-06555-x)]

**The Shaky Foundations of Large Language Models and Foundation Models for Electronic Health Records.** [2023].<br>
*M. Wornow, Y. Xu, R. Thapa, B. Patel et al.*<br>
npj Digital Medicine, vol. 6, pp. 135.<br>
[[PDF](https://doi.org/10.1038/s41746-023-00879-8)]

**Clinical, Cultural, Computational, and Regulatory Considerations to Deploy AI in Radiology: A Review and Call to Action.** [2024].<br>
*M. G. Linguraru et al.*<br>
Radiology: Artificial Intelligence, vol. 6(4), pp. e240225.<br>
[[PDF](https://doi.org/10.1148/ryai.240225)]

---

# Statistical & Evaluation Methods

**Meta-analysis in clinical trials.** [1986].<br>
*R. DerSimonian, N. Laird.*<br>
Controlled Clinical Trials, vol. 7(3), pp. 177–188.<br>
[[PDF](https://doi.org/10.1016/0197-2456(86)90046-2)]

**Comparing images using the Hausdorff distance.** [1993].<br>
*D. P. Huttenlocher, G. A. Klanderman, W. J. Rucklidge.*<br>
IEEE Transactions on Pattern Analysis and Machine Intelligence, vol. 15(9), pp. 850–863.<br>
[[PDF](https://doi.org/10.1109/34.232073)]

**Measuring inconsistency in meta-analyses.** [2003].<br>
*J. P. T. Higgins, S. G. Thompson, J. J. Deeks, D. G. Altman.*<br>
BMJ, vol. 327(7414), pp. 557–560.<br>
[[PDF](https://doi.org/10.1136/bmj.327.7414.557)]

**Elements of Information Theory.** [2006].<br>
*T. M. Cover, J. A. Thomas.*<br>
2nd edition, Wiley-Interscience.<br>
[[PDF](https://doi.org/10.1002/047174882X)]

**Recommendations for examining and interpreting funnel plot asymmetry in meta-analyses of randomised controlled trials.** [2011].<br>
*J. A. C. Sterne, A. J. Sutton, J. P. A. Ioannidis, N. Terrin, D. R. Jones et al.*<br>
BMJ, vol. 343, pp. d4002.<br>
[[PDF](https://doi.org/10.1136/bmj.d4002)]

**The PRISMA 2020 statement: an updated guideline for reporting systematic reviews.** [2021].<br>
*M. J. Page, J. E. McKenzie, P. M. Bossuyt, I. Boutron, T. C. Hoffmann, C. D. Mulrow et al.*<br>
BMJ, vol. 372, pp. n71.<br>
[[PDF](https://doi.org/10.1136/bmj.n71)]

---

## Citation

If you find this repository useful for your research, please cite our survey:

```bibtex
@article{masood2026alsd_vlm_review,
  author  = {Rao Farhat Masood and Imtiaz Ahmad Taj},
  title   = {Automated Lumbar Spine Diagnostics via Vision--Language Foundation Models: A Systematic Mathematical Review of Architectures, Distillation Strategies and Clinical Deployment Pathways},
  journal = {TBD},
  year    = {2026},
  note    = {Under-Finalization}
}
```

---

<!-- ## Contact

For any questions or suggestions, please open an issue or contact [Rao Farhat Masood](mailto:farhatmasood.fm@gmail.com). -->

---

## Star History

If you find this work helpful, please consider giving it a ⭐!
