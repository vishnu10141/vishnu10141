<div align="center">

<img src="./assets/hero.svg" width="100%" alt="Vishnu Nimmakayala — ML Engineer"/>

</div>

<div align="left">
  <a href="https://vishnu-ai-portfolio-864n.vercel.app"><img src="./assets/hero-btn-portfolio.svg" width="17.77%" alt="Portfolio"></a><a href="https://github.com/vishnu10141"><img src="./assets/hero-btn-github.svg" width="14.66%" alt="GitHub"></a>
</div>


<div align="center">

<img src="./assets/divider.svg" width="100%" alt=""/>

</div>


<div align="center">

<img src="https://readme-typing-svg.demolab.com/?font=JetBrains+Mono&weight=400&size=11&duration=3000&pause=800&color=4F8FFF&center=true&vCenter=true&width=500&height=22&lines=ML+Engineer+%C2%B7+AI+Developer;Computer+Vision+%C2%B7+Medical+Imaging;NLP+%C2%B7+Deep+Learning+%C2%B7+Defense+ML" alt="role-typing"/>

</div>


> CS&amp;E graduate (2026) working on machine learning and applied AI. Interned at **DRDO** on radar signal classification and at **IIIT Hyderabad** on Telugu NLP corpus development. Building projects across computer vision, NLP, and deep learning — from training to deployment.


<div align="center">

<img src="./assets/divider.svg" width="100%" alt=""/>

</div>


<!--
================================================================
  TIMELINE
================================================================
-->

<div align="center">

<img src="./assets/timeline.svg" width="100%" alt="Career Timeline"/>

</div>


<div align="center">

<img src="./assets/divider.svg" width="100%" alt=""/>

</div>


<!--
================================================================
  INTERNSHIPS
================================================================
-->

<div align="center">

<sub><b>INTERNSHIPS</b></sub>

</div>


<details>
<summary><img src="./assets/experience-drdo.svg" width="100%" alt="DRDO — ML Intern"/></summary>


<div align="center">

**ML Intern — DRDO, Hyderabad** &nbsp;`2023`

</div>


**Problem**

Operational radar systems generate false detections due to electronic countermeasure (ECM) jamming. These false targets degrade situational awareness and can lead to critical decision errors in defense scenarios. A reliable automated system was needed to distinguish genuine radar returns from manufactured interference.

**Responsibilities**

- Analyzed raw radar return data and designed feature extraction pipelines for time-domain signal characteristics
- Engineered discriminative features including signal energy, pulse width distribution, Doppler spread, and spectral signatures
- Trained and evaluated ensemble classifiers — XGBoost, Random Forest, SVM — on labeled defense-grade datasets
- Iteratively improved model generalization through cross-validation and threshold tuning

**Outcome**

- Achieved high-precision binary classification of radar targets vs. false ECM-induced detections
- Delivered a reproducible ML pipeline suitable for integration into signal processing workflows
- Produced interpretable feature importance rankings enabling domain expert validation


<div align="center">

`Signal Processing` &nbsp; `XGBoost` &nbsp; `Random Forest` &nbsp; `SVM` &nbsp; `Feature Engineering` &nbsp; `Scikit-learn` &nbsp; `NumPy`

</div>

</details>


<details>
<summary><img src="./assets/experience-iiit.svg" width="100%" alt="IIIT Hyderabad — NLP Intern"/></summary>


<div align="center">

**NLP Intern — IIIT Hyderabad** &nbsp;`2022`

</div>


**Problem**

South Indian languages like Telugu are critically under-resourced in NLP. The absence of large, high-quality annotated corpora prevents training of robust language models for over 82 million native speakers.

**Responsibilities**

- Contributed to structured Telugu NLP dataset design and curation for low-resource language modelling
- Performed manual linguistic annotation across morphological, syntactic, and semantic dimensions
- Worked under supervision to ensure annotation consistency and inter-annotator agreement
- Helped build corpus pipelines for text normalization, tokenization, and structured data storage

**Outcome**

- Produced annotated linguistic data contributing to Telugu language model infrastructure
- Corpus resources support downstream NLP tasks: POS tagging, NER, parsing, and text classification


<div align="center">

`Low-Resource NLP` &nbsp; `Dataset Annotation` &nbsp; `Corpus Construction` &nbsp; `Telugu Language` &nbsp; `Linguistic Annotation`

</div>

</details>


<div align="center">

<img src="./assets/divider.svg" width="100%" alt=""/>

</div>


<!--
================================================================
  PROJECTS
================================================================
-->

<div align="center">

<sub><b>FEATURED PROJECTS</b></sub>

</div>


<details>
<summary>

<div align="center">

**Brain Tumor Detection &amp; Segmentation** &nbsp;·&nbsp; <sub>Medical Imaging · 3D Deep Learning · Explainable AI</sub>

</div>

</summary>


<div align="center">

<a href="https://github.com/vishnu10141/Brain-Tumor-Detection-and-Segmentation"><img src="./assets/project-tumor.svg" width="100%" alt="Brain Tumor Detection — Architecture"/></a>

</div>


**Problem**

Brain tumor segmentation from multi-modal MRI is inherently complex: tumors exhibit high variability in shape, size, and appearance across T1, T2, FLAIR, and T1ce modalities. Clinical deployment further requires model predictions to be interpretable by radiologists — not just accurate.

**Solution**

A 3D Residual Attention U-Net trained on the BraTS 2020 benchmark dataset for multi-class segmentation of enhancing tumor, tumor core, and whole tumor regions across four MRI modalities. Grad-CAM++ saliency maps provide region-level visual explanations, and a Streamlit dashboard surfaces model output in a clinical interface.

**Pipeline**

`MRI Input` → `MONAI Preprocessing` → `3D Res-Attn U-Net` → `Multi-class Segmentation` → `Grad-CAM++ Explainability` → `Streamlit Dashboard`

**Challenges**

- Class imbalance between tumor sub-regions and healthy tissue across 3D volumes
- Maintaining spatial context across all three dimensions with efficient GPU memory usage
- Making model predictions legible to clinical users without deep ML expertise

**Outcome**

- Strong Dice scores across tumor sub-regions on BraTS 2020 validation split
- Explainability layer enabling verification of model predictions
- End-to-end deployable system from raw MRI DICOM to annotated segmentation output


<div align="center">

`PyTorch` &nbsp; `3D U-Net` &nbsp; `Residual Attention` &nbsp; `Grad-CAM++` &nbsp; `BraTS 2020` &nbsp; `MONAI` &nbsp; `Streamlit`

</div>

</details>


<details>
<summary>

<div align="center">

**Radar False Target Detection** &nbsp;·&nbsp; <sub>Defense ML · Signal Intelligence · Ensemble Classifiers</sub>

</div>

</summary>


<div align="center">

<img src="./assets/project-radar.svg" width="100%" alt="Radar Detection — Signal Classification"/>

</div>


**Problem**

Modern radar systems face sophisticated electronic countermeasures that inject synthetic false targets — ghost echoes — into the return signal. Without automated discrimination, operators face an overwhelming volume of alerts, compromising response time and mission effectiveness.

**Solution**

An ML classification pipeline that ingests raw radar return data, applies targeted feature engineering at the signal processing level, and deploys an ensemble of classifiers (XGBoost, Random Forest, SVM) to distinguish genuine targets from ECM-induced false detections.

**Pipeline**

`Radar Signal Data` → `Signal Processing` → `Feature Engineering` → `Ensemble Classifiers` → `Binary Classification Output`

**Technologies**

`XGBoost` &nbsp; `Random Forest` &nbsp; `SVM` &nbsp; `Scikit-learn` &nbsp; `NumPy` &nbsp; `Signal Processing`

**Outcome**

- High-accuracy binary classification of radar targets vs. false ECM returns
- Interpretable feature importances enabling validation by domain experts
- Modular pipeline architecture suitable for real-time integration


<sub><i>Repository not publicly available — developed during DRDO internship on classified datasets.</i></sub>

</details>


<details>
<summary>

<div align="center">

**Telugu LLM — Chandamama Kathalu** &nbsp;·&nbsp; <sub>NLP · LLM · Telugu Language</sub>

</div>

</summary>


<div align="center">

<img src="./assets/project-llm.svg" width="100%" alt="Telugu LLM — Chandamama Kathalu"/>

</div>


**Overview**

Building a language model trained on Chandamama Kathalu, a classic Telugu children's stories corpus. The project focuses on low-resource language modeling for Telugu — a language with limited NLP tooling — using a domain-specific text corpus.

**Pipeline**

`Data Collection` → `Text Preprocessing` → `Custom Tokenization` → `Model Training` → `Telugu Text Generation`

**Approach**

- Curated and preprocessed Chandamama Kathalu stories as the training corpus
- Built a custom Telugu tokenizer suited to the script and morphology
- Trained a language model for text generation and story completion


<div align="center">

`Python` &nbsp; `HuggingFace` &nbsp; `PyTorch` &nbsp; `Transformers` &nbsp; `Telugu NLP` &nbsp; `Tokenization`

</div>

</details>


<div align="center">

<img src="./assets/divider.svg" width="100%" alt=""/>

</div>


<!--
================================================================
  TECH STACK
================================================================
-->

<div align="center">

<sub><b>TECHNICAL ECOSYSTEM</b></sub>

</div>


<div align="center">

<img src="./assets/skills.svg" width="100%" alt="Tech Stack — AI Ecosystem"/>

</div>


<div align="center">

<img src="./assets/divider.svg" width="100%" alt=""/>

</div>


<!--
================================================================
  CONTACT
================================================================
-->

<div align="center">

<sub><b>GET IN TOUCH</b></sub>

</div>


<div align="center">

<a href="https://vishnu-ai-portfolio-864n.vercel.app"><img src="./assets/contact-portfolio.svg" width="24%" alt="Portfolio"></a>
<a href="https://github.com/vishnu10141"><img src="./assets/contact-github.svg" width="24%" alt="GitHub"></a>
<a href="https://www.linkedin.com/in/vishnu-nimmakayala-8a41021b4/"><img src="./assets/contact-linkedin.svg" width="24%" alt="LinkedIn"></a>
<a href="mailto:nvishnu1014@gmail.com"><img src="./assets/contact-email.svg" width="24%" alt="Email"></a>

</div>


<div align="center">

<img src="./assets/footer.svg" width="100%" alt=""/>

</div>
