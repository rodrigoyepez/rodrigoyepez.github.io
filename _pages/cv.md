---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

## Education

**M.S. Computer Science** — University of Maryland, Baltimore County  
*May 2025* | GPA: 3.6/4.0

**B.S. Computer Science** — American University  
*May 2023*

---

## Work Experience

**General Associate**  
UMBC, Division of Information Technology — Baltimore, MD  
*May 2025 – Present*

- Lead development of real-time transcription and visualization pipelines (Linux, SQL, Python, LLMs, AWS Redshift, Tableau, Power BI) to analyze classroom conversations and support research on effective classroom interactions
- Collaborate with cross-functional Agile teams to troubleshoot and optimize deployed AI solutions

**Graduate Research Assistant**  
UMBC, College of Engineering and Technology — Baltimore, MD  
*August 2023 – May 2025*

- Architected multimodal AI systems integrating audio and text data through feature extraction, improving dementia classification accuracy
- Built and maintained a 10TB SQL database to improve multi-omics data analysis and AI cancer classification
- Collaborated weekly with cross-disciplinary teams to align technical solutions with research and business needs
- Documented technical processes to ensure reproducibility, accessibility, and compliance across research workflows

**Undergraduate Research Assistant**  
American University, Big Data Lab — Washington, D.C.  
*September 2021 – May 2023*

- Developed scalable pipelines using NASA imagery with Linux, Python, SQL, and Spark, improving cloud classification by 20%
- Designed and implemented LSTM model on medical signal data to predict lung recovery up to 8 hours in advance
- Built real-time MLOps data drift monitoring system with Python, TensorFlow, and Spark to detect shifts and auto-trigger model retraining

**Research Intern**  
Big Data REU, UMBC — Baltimore, MD  
*June 2021 – August 2021*

- Optimized compact neural networks through hyperparameter search, reducing parameters by 30% while maintaining accuracy
- Benchmarked model performance and created visualizations to communicate results to technical stakeholders

---

## Skills

| Category | Technologies |
|----------|-------------|
| **Programming** | Python, SQL, C++, Pandas, Git, Docker, REST APIs |
| **ML Frameworks** | PyTorch, Keras, Scikit-Learn, PySpark, AWS |
| **Deep Learning** | CNNs, Transformers, Object Detection, Segmentation, NeRFs |
| **Soft Skills** | Agile Development, Technical Documentation, Cross-Functional Teamwork |
| **Languages** | English, Spanish, French (Fluent) |

---

## Publications

<ul>{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}</ul>