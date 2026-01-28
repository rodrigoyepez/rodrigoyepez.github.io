---
title: "Distributed Concept Drift Detection for Efficient Model Adaptation with Big Data Streams"
collection: publications
category: conferences
permalink: /publication/2023-distributed-drift-detection
excerpt: 'Distributed drift detection workflow using DDM algorithm with Apache Spark for scalable model adaptation.'
date: 2023-12-15
venue: '2023 IEEE International Conference on Big Data'
paperurl: 'https://doi.org/10.1109/BigData59044.2023.10386334'
citation: 'I. Whitehouse, R. Yepez-Lopez, R. Corizzo. (2023). &quot;Distributed Concept Drift Detection for Efficient Model Adaptation with Big Data Streams.&quot; <i>IEEE Big Data 2023</i>.'
---

We propose a distributed drift detection workflow based on the DDM algorithm paired with a Random Forest predictive model, implemented in Apache Spark. The workflow adaptively updates models as drifts are detected, leveraging Pandas UDFs for efficient distribution across multiple worker nodes. Experiments on two real-world datasets demonstrate positive results in Speedup, Scaleup, and detection delay compared to single-node implementations.