<div align="center">

<img src="./assets/hero.svg" width="100%" alt="Vishnu Nimmakayala — AI Engineer"/>

</div>

<div align="left">
  <a href="https://vishnu-ai-portfolio-864n.vercel.app"><img src="./assets/hero-btn-portfolio.svg" width="18.66%" alt="Portfolio"></a><a href="https://github.com/vishnu10141"><img src="./assets/hero-btn-github.svg" width="14.66%" alt="GitHub"></a>
</div>


<div align="center">

<img src="./assets/particles.svg" width="100%" alt=""/>

</div>

<div align="center">

<img src="./assets/divider-1.svg" width="100%" alt=""/>

</div>


<!--
================================================================
  ABOUT
================================================================
-->

<div align="center">

<img src="https://readme-typing-svg.demolab.com/?font=JetBrains+Mono&weight=400&size=11&duration=3000&pause=800&color=3B82F6&center=true&vCenter=true&width=500&height=22&lines=AI+Engineer+%C2%B7+Machine+Learning+Researcher;Computer+Vision+%C2%B7+Medical+Imaging;Natural+Language+Processing+%C2%B7+Defense+ML" alt="role-typing"/>

</div>


> Computer Science & Engineering graduate building interpretable AI systems at the intersection of deep learning, computer vision, and medical imaging. Research experience spans signal classification at **DRDO** and low-resource NLP corpus development at **IIIT Hyderabad**. Work covers the full deep learning lifecycle — architecture design through production deployment — with emphasis on clinical explainability and real-world operational grounding.


<div align="center">

<img src="./assets/neural-grid.svg" width="100%" alt=""/>

</div>


<div align="center">

<img src="./assets/divider-2.svg" width="100%" alt=""/>

</div>


<!--
================================================================
  TIMELINE
================================================================
-->

<div align="center">

<img src="./assets/timeline.svg" width="100%" alt="Research Timeline"/>

</div>


<div align="center">

<img src="./assets/divider-3.svg" width="100%" alt=""/>

</div>


<!--
================================================================
  EXPERIENCE
================================================================
-->

<div align="center">

<sub><b>RESEARCH EXPERIENCE</b></sub>

</div>


<details>
<summary><img src="./assets/experience-drdo.svg" width="100%" alt="DRDO — Machine Learning Research Intern"/></summary>


<div align="center">

**Machine Learning Research Intern — DRDO, Hyderabad** &nbsp;`2023`

</div>


**Problem**

Operational radar systems generate false detections due to electronic countermeasure (ECM) jamming. These false targets degrade situational awareness and can lead to critical decision errors in defense scenarios. A reliable automated system was needed to distinguish genuine radar returns from manufactured interference.

**Responsibilities**

- Analyzed raw radar return data and designed feature extraction pipelines for time-domain signal characteristics
- Engineered discriminative features including signal energy, pulse width distribution, Doppler spread, and spectral signatures
- Trained and evaluated ensemble classifiers — XGBoost, Random Forest, SVM — on labeled defense-grade datasets
- Iteratively improved model generalization through cross-validation and threshold tuning

**Impact**

- Achieved high-precision binary classification of radar targets vs. false ECM-induced detections
- Delivered a reproducible ML pipeline suitable for integration into signal processing workflows
- Produced interpretable feature importance rankings enabling domain expert validation


<div align="center">

`Signal Processing` &nbsp; `XGBoost` &nbsp; `Random Forest` &nbsp; `SVM` &nbsp; `Feature Engineering` &nbsp; `Scikit-learn` &nbsp; `NumPy`

</div>

</details>


<details>
<summary><img src="./assets/experience-iiit.svg" width="100%" alt="IIIT Hyderabad — NLP Research Intern"/></summary>


<div align="center">

**NLP Research Intern — IIIT Hyderabad** &nbsp;`2023`

</div>


**Problem**

South Indian languages like Telugu are critically under-resourced in NLP. The absence of large, high-quality annotated corpora prevents training of robust language models for over 82 million native speakers.

**Responsibilities**

- Contributed to structured Telugu NLP dataset design and curation for low-resource language modelling
- Performed manual linguistic annotation across morphological, syntactic, and semantic dimensions
- Worked under research supervision to ensure annotation consistency and inter-annotator agreement
- Helped build corpus pipelines for text normalization, tokenization, and structured data storage

**Impact**

- Produced annotated linguistic data contributing to Telugu language model research infrastructure
- Corpus resources directly support downstream NLP tasks: POS tagging, NER, parsing, and text classification


<div align="center">

`Low-Resource NLP` &nbsp; `Dataset Annotation` &nbsp; `Corpus Construction` &nbsp; `Telugu Language` &nbsp; `Linguistic Annotation`

</div>

</details>


<div align="center">

<img src="./assets/divider-4.svg" width="100%" alt=""/>

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

**Brain Tumor Detection & Segmentation** &nbsp;·&nbsp; <sub>Medical Imaging · 3D Deep Learning · Explainable AI</sub>

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
- Clinically-oriented explainability layer enabling radiologist trust and verification
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

An ML classification pipeline that ingests raw radar return data, applies targeted feature engineering at the signal processing level, and deploys an ensemble of classifiers (XGBoost, Random Forest, SVM) to distinguish genuine targets from ECM-induced false detections with high precision and interpretable confidence scores.

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

**AI Portfolio Website** &nbsp;·&nbsp; <sub>Next.js · Vercel · Full-Stack</sub>

</div>

</summary>


<div align="center">

<a href="https://vishnu-ai-portfolio-864n.vercel.app"><img src="./assets/project-portfolio.svg" width="100%" alt="Portfolio Website — Architecture"/></a>

</div>


**Overview**

A fully responsive personal portfolio designed for clarity, speed, and professional presentation. Built with Next.js App Router, deployed on Vercel's global edge network. Showcases research work, featured projects, and technical background with smooth animations and dark-mode-first design.

**Architecture**

`Next.js 14 (App Router)` → `Vercel Edge Deploy` → `Global CDN` → `User`

**Features**

- Responsive layout across mobile, tablet, and desktop viewports
- Dark mode native design with animated transitions
- Optimized Core Web Vitals — LCP, FID, CLS targets achieved
- Project showcase with dynamic routing and rich media support


<div align="center">

`Next.js` &nbsp; `JavaScript` &nbsp; `CSS` &nbsp; `Vercel` &nbsp; `React`

</div>

</details>


<div align="center">

<img src="./assets/divider-5.svg" width="100%" alt=""/>

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

<img src="./assets/stack-diagram.svg" width="100%" alt="Tech Stack — AI Ecosystem"/>

</div>


<div align="center">
<table>
<tr>
<td align="center" width="25%">

**Core Language**

Python 3.11+

</td>
<td align="center" width="25%">

**Deep Learning**

PyTorch · TensorFlow · MONAI

</td>
<td align="center" width="25%">

**Computer Vision**

OpenCV · Grad-CAM++ · PIL

</td>
<td align="center" width="25%">

**NLP**

HuggingFace · spaCy · NLTK

</td>
</tr>
<tr>
<td align="center">

**ML**

Scikit-learn · XGBoost · SVM

</td>
<td align="center">

**Data**

NumPy · Pandas · Matplotlib

</td>
<td align="center">

**Deployment**

FastAPI · Streamlit · Docker

</td>
<td align="center">

**Stack**

Next.js · Linux · Git · Vercel

</td>
</tr>
</table>
</div>


<div align="center">

<img src="./assets/divider-6.svg" width="100%" alt=""/>

</div>


<!--
================================================================
  CURRENTLY EXPLORING
================================================================
-->

<div align="center">

<sub><b>CURRENTLY EXPLORING</b></sub>

</div>


<div align="center">

<code>vishnu@research:~$</code>


<img src="https://readme-typing-svg.demolab.com/?font=JetBrains+Mono&weight=400&size=14&duration=2800&pause=900&color=38BDF8&center=true&vCenter=true&width=580&height=30&lines=%3E+Explainable+AI+for+clinical+medical+imaging;%3E+3D+multi-modal+segmentation+pipelines;%3E+Instruction-tuned+LLM+domain+adaptation;%3E+Reproducible+MLOps+%2B+experiment+tracking;%3E+Foundation+models+for+medical+vision" alt="currently-exploring"/>

</div>


<div align="center">

<img src="./assets/background.svg" width="100%" alt=""/>

</div>


<div align="center">

<img src="./assets/divider-7.svg" width="100%" alt=""/>

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
