---
title: Accepted Papers
layout: default
---

# Accepted Papers

The accepted papers were peer-reviewed by the SSDBM 2024 technical program committees. From the submissions the committee selected 11 full research papers, 7 short research papers, and 1 demonstration paper.

## Accepted Long Research Papers

**Model Reuse in Learned Spatial Indexes**

_Mayur Patil (University of California, Riverside, USA) and Chinya V Ravishankar (University of California, Riverside, USA)._

Abstract

Learned database indexes use machine learning algorithms to directly predict the location of a query key within a sorted key array, thereby eliminating index search overhead. Prior work shows learned indexes outperforming traditional indexes in both space and query time for one-dimensional data, especially for read-intensive workloads. Usually, learned indexes linearize the multi-dimensional data with a space-filling curve before generating the index.
However, learned indexes can have very high build times. Multi-level models are often needed, since a single model built for the
entire dataset has low accuracy. The total number of models is often large, drastically increasing model build time.
We present a new approach to these challenges called Learned Spatial Indexing with model Reuse (LSIR) that dramatically reduces learned index training time, via model reuse. We first adaptively partition the dataset into cells, and form clusters of cells with similar data distributions. We next build a “seed” model for each cluster, and tune it for each cell in the cluster. Our experiments on large datasets and query workloads, both real-world and synthetic, show that our approach reduces build time by more than 90% compared to traditional learned spatial indexes, with improved model accuracy. LSIR also reduces query response time by 80%, 40%, and 52% for point, range, and kNN queries respectively.


**The Intersection of Compliance, Databases, and IT Operations.**

_Ben Lenard (Argonne National Laboratory,DePaul University), Alexander Rasin (DePaul University), Nick Scope (DePaul University) and Thamer Al Johani (DePaul University). ._ 

Abstract

Most organizations rely on a relational database(s) for their day-to- day business functions. Data management policies fall under the umbrella of IT Operations, dictated by a combination of internal organizational policies and government regulations. Many privacy laws (such as Europe’s General Data Protection Regulation and California’s Consumer Privacy Act) establish policy requirements for organizations, requiring the preservation or purging of certain customer data across their systems. Organization disaster recovery policies also mandate backup policies to prevent data loss. Thus, the data in these databases are subject to a range of policies, including data retention and data purging rules, which may come into conflict with the need for regular backups.
In this paper, we discuss the trade-offs between different compliance mechanisms to maintain IT Operational policies. We consider the practical availability of data in an active relational database and in a backup, including: 1) supporting data privacy rules with re- spect to preserving or purging customer data, and 2) the application performance impact caused by the database policy implementation. We first discuss the state of data privacy compliance in database systems. We then look at enforcement of common IT operational policies with regard to database backups. We consider different implementations used to enforce privacy rule compliance combined with a detailed discussion for how these approaches impact the performance of a database at different phases. We demonstrate that naive compliance implementations will incur a prohibitively high cost and impose onerous restrictions on backup and restore process, but will not affect daily user query transaction cost. However, we also show that other solutions can achieve a far lower backup and restore costs at a price of a small (<5%) overhead to non-SELECT queries.


**Similarity Measures Recommendation for Mixed Data Clustering.**

_Abdoulaye Diop (IRIT), Nabil El Malki (IRIT), Max Chevalier (IRIT), André Péninou (IRIT), Roman Jimenez Geoffrey (SolutionData Group) and Olivier Teste (IRIT)._ 

Abstract

Clustering is an important data mining task which is widely spread in various domains such as biology, finance, marketing, healthcare, and social sciences. It allows the end user to discover, through built clusters, relationships within data. Many non-expert users perceive clustering as an "easy" task because it always produces a result. However, choosing a clustering algorithm at random, without proper parameter tuning, often leads to poor results.
In particular, an important choice when applying a clustering algorithm to a specific dataset is the similarity measure. Since clustering algorithms rely on similarities between data points to build clusters, the chosen similarity measure should fit the data as accurately as possible in order to form the best clusters.
Mixed Data are data that are characterized by numerical as well as categorical attributes. When clustering mixed data, the same similarity measure cannot be used for the two attribute types. Commonly a pair of similarity measures is used, one dedicated to numerical attributes and one dedicated to categorical attributes. The choice of these two most appropriate similarity measures is very important in mixed data, as it significantly affects the clustering performance.
In this paper, we challenge to recommend the best pairs of similarity measures to end-users, regardless of their experience, when applying a specific clustering algorithm to a mixed dataset to maximize a specific performance measure. The proposed recommendation process relies on knowledge extracted from a meta-model built by an automated machine learning (AutoML) approach. To evaluate the relevance of the recommendation process, experiments are conducted with two well-known clustering algorithms: K-Prototypes and Hierarchical Clustering. Our results show that the recommendations can positively help users select the most appropriate pairs of similarity measures depending on their use cases (i.e. clustering algorithm, dataset, and performance measure). These recommendations outperform the traditionally used similarity measures in the literature, particularly for datasets where the choice of the similarity measures has a significant impact.


**CURD: Context-aware Relevance and Urgency Determination**

_Ademola Adesokan (Missouri University of Science and Technology) and Sanjay Madria (Missouri University of Science and Technology)._ 

Abstract

During emergencies where time is of the essence, efficient management of disasters depends on swiftly recognizing relevant and urgent information from online platforms like X (Twitter), which is imperative for augmenting established response frameworks, such as the 911 emergency system. This paper introduces CURD, a Contextual-aware Relevance and Urgency Determination system designed to enhance the efficiency of disaster response. The system addresses two critical challenges: filtering out irrelevant data and assessing the urgency of relevant information. Our approach includes a multi-level annotation process for event type, relevancy, and an urgency annotation algorithm that significantly improves information extraction accuracy and efficiency. CURDdl, our classifier, uses a deep learning pipeline architecture with a combination of transformer models, a convolution layer, and custom attention mechanisms to classify disaster-related tweets into multiclass-event type, binary-relevance-and-urgency categories, and rank urgent ones based on significance. Experimental results show that our best baseline classifiers for all three tasks achieved ≥ 88% F1 and accuracy, and ≥ 94%. AUC. Our models also outperformed models from related works in all metrics, validating the effectiveness of CURD in prioritizing response messages that will facilitate decision-making and resource allocation in disaster scenarios. CURD annotated dataset and code are available on CURD Dataset and Code.


**Imbalanced Graph-Level Anomaly Detection via Counterfactual Augmentation and Feature Learning**

_Zitong Wang (School of Cyber Science and Engineering, Wuhan University), Xuexiong Luo (School of Computing, Macquarie University), Enfeng Song (Renmin Hospital of Wuhan University), Qiuqing Bai (School of Cyber Science and Engineering, Wuhan University) and Fu Lin (School of Computer Science, Wuhan University, School of Cyber Science and Engineering, Wuhan University)._ 

Abstract

Graph-level anomaly detection (GLAD) has already gained significant importance and has become a popular field of study, attracting considerable attention across numerous downstream works. The core focus of this domain is to capture and highlight the anomalous information within given graph datasets. In most existing studies, anomalies are often the instances of few. The stark imbalance misleads current GLAD methods to focus on learning the patterns of normal graphs more, further impacting anomaly detection performance. Moreover, existing methods predominantly utilize the inherent features of nodes to identify anomalous graph patterns which is approved suboptimal according to our experiments. In this work, we propose an imbalanced GLAD method via counterfactual augmentation and feature learning. Specifically, we first construct anomalous samples based on counterfactual learning, aiming to expand and balance the datasets. Additionally, we construct a module based on Graph Neural Networks (GNNs), which allows us to utilize degree attributes to complement the inherent attribute features of nodes. Then, we design an adaptive weight learning module to integrate features tailored to different datasets effectively to avoid indiscriminately treating all features as equivalent. Furthermore, extensive baseline experiments conducted on public datasets substantiate the robustness and effectiveness. Besides, we apply the model to brain disease datasets, which can prove the generalization capability of our work. The source code of our work is available online.


**A Compact and Efficient Neural Data Structure for Mutual Information Estimation in Large Timeseries**

_Fatemeh Farokhmanesh (Technical University of Munich), Christoph Neuhauser (Technical University of Munich) and Rüdiger Westermann (Technical University of Munich)._ 

Abstract

Database systems face challenges when using mutual information (MI) for analyzing non-linear relationships between large timeseries, due to computational and memory requirements. Interactive workflows are especially hindered by long response times. To address these challenges, we present timeseries neural MI fields (TNMIFs), a compact data structure that has been trained to reconstruct MI efficiently across various time-windows and window positions in large timeseries. We demonstrate learning and reconstruction with a large timeseries dataset comprising 1420 timeseries, each storing data at 1639 timesteps. While the learned data structure consumes only 45 megabytes, it answers queries for the MI estimates between the windows in a selected timeseries and the corresponding windows in all other timeseries within 44 milliseconds. Given a measure of similarity between timeseries based on windowed MI estimates, even the matrix showing all mutual timeseries similarities can be computed in less than 32 seconds. To support measuring dependence between lagged timeseries, an extended data structure learns to reconstruct MI to positively (future) and negatively (past) lagged windows. Using a maximum lag of 64 in both directions decreases query times by about a factor of 10.

**AI Data Readiness Inspector (AIDRIN) for Quantitative Assessment of Data Readiness for AI**

_Kaveen Hiniduma (The Ohio State University), Suren Byna (The Ohio State University), Jean Luca Bez (Lawrence Berkeley National Laboratory) and Ravi Madduri (Argonne National Laboratory)._ 

Abstract

Garbage In Garbage Out is a universally agreed quote by computer scientists from various domains, including Artificial Intelligence (AI). As data is the fuel for AI, models trained on low-quality, biased data are often ineffective. Computer scientists who use AI invest a considerable amount of time and effort in preparing the data for AI. However, there are no standard methods or frameworks for assessing the “readiness” of data for AI. To provide a quantifiable assessment of the readiness of data for AI processes, we define parameters of AI data readiness and introduce AIDRIN (AI Data Readiness INspector). AIDRIN is a framework covering a broad range of readiness dimensions available in the literature that aid in evaluating the readiness of data quantitatively and qualitatively. AIDRIN uses metrics in traditional data quality assessment such as completeness, outliers, and duplicates for data evaluation. Furthermore, AIDRIN uses metrics specific to assess data for AI, such as feature importance, feature correlations, class imbalance, fairness, privacy, and FAIR (Findability, Accessibility, Interoperability, and Reusability) principle compliance. AIDRIN provides visualizations and reports to assist data scientists in further investigating the readiness of data. The AIDRIN framework enhances the efficiency of the machine learning pipeline to make informed decisions on data readiness for AI applications.

**Statistical Privacy and Consent in Data Aggregation**

_Nick Scope (DePaul University), Alexander Rasin (DePaul University), Ben Lenard (Argonne National Laboratory,DePaul University) and James Wagner (University of New Orleans)._ 

Abstract

As new laws governing management of personal data are introduced, e.g., the European Union’s General Data Protection Regulation of 2016 and the California Consumer Privacy Act of 2018, compliance with data governance legislation is becoming an increasingly important aspect of data management. An important component of many data privacy laws is that they require companies to only use an individual's data for a purpose the individual has explicitly consented to. Prior methods for enforcing consent for aggregate queries either use access control to eliminate data without consent from query evaluation or apply differential privacy algorithms to inject synthetic noise into the outcomes of queries (or input data) to ensure that the anonymity of non-consenting individuals is preserved with high probability. Both approaches return query results that differ from the ground truth results corresponding to the full input containing data from both consenting and non-consenting individuals. We present an alternative framework for group-by aggregate queries, tailored for applications, e.g., medicine, where even a small deviation from the correct answer to a query cannot be tolerated. Our approach uses provenance to determine, for each output tuple of a group-by aggregate query, which individual's data was used to derive the result for this group. We then use statistical tests to determine how likely it is that the presence of data for a non-consenting individual will be revealed by such an output tuple. We filter out tuples for which this test fails, i.e., which are deemed likely to reveal non-consenting data. Thus, our approach always returns a subset of the ground truth query answers. Our experiments successfully return only 100\% accurate results in instances where access control or differential privacy would have either returned less total or less accurate results.

**Scale Fairness on Spectral Clustering**

_Zhijing Yang (Southwest University of Science and Technology), Hui Zhang (Southwest University of Science and Technology), Chunming Yang (School of Computer Science and Technology, Southwest University of Science and Technology), Bo Li (School of Computer Science and Technology, Southwest University of Science and Technology), Xujian Zhao (Southwest University of Science and Technology) and Yin Long (Southwest University of Science and Technology)._ 

Abstract

The fairness and bias of spectral clustering algorithms have attracted considerable research interest in recent years. Currently, fair spectral clustering algorithms are based on the notions of group fairness and individual fairness, which effectively reduce decision bias for similar individuals and sensitive groups. Existing fair spectral clustering algorithms achieve a certain degree of resource redistribution during the clustering process for a particular individual or part of a group, but there is still a situation where the final decision is unfair to the oversized or undersized result clusters. To this end, we present the first principled study of Scale Fairness on Spectral Clustering and propose the SFSC algorithm, which aims to effectively reduce the possibility of the results being oversized or undersized clusters by introducing entropy computation into the spectral clustering process. We measure the scale fairness of clusters by two statistical metrics and demonstrate on eight classical and real-world datasets that SFSC has better fairness performance compared to spectral clustering while having a comparable clustering effect. To the best of our knowledge, this paper is the first study to propose scale fairness for spectral clustering.

**How do users design scientific workflows? The Case of Snakemake and Nextflow**

_Sebastian Pohl (Humboldt-Universität zu Berlin), Nourhan Elfaramawy (Humboldt-Universität zu Berlin), Artur Miling (Humboldt-Universität zu Berlin), Kedi Cao (Leibniz Institute for Immunotherapy), Birte Kehr (Leibniz Institute for Immunotherapy) and Matthias Weidlich (Humboldt-Universität zu Berlin)._ 

Abstract

Scientific workflows automate the analysis of large-scale scientific data, fostering the reuse of data processing operators as well as the reproducibility and traceability of analysis results. In exploratory research, however, workflows are continuously adapted, utilizing a wide range of tools and software libraries, to test scientific hypotheses. Script-based workflow engines cater to the required flexibility through direct integration of programming primitives, but lack abstractions for interactive exploration of the workflow design by a user during workflow execution.
In this paper, we study the requirements for the design of interactive workflows through the lens of existing workflow collections. Specifically, we focus on two widely used script-based workflow engines: Snakemake and Nextflow. For Snakemake, we collected workflows from 1602 GitHub repositories that are listed in the Snakemake workflow catalog. For Nextflow, we adopted the nf-core collection with workflows from 94 GitHub repositories as the basis for our study. Using these collections, we present insights on common structures in the design of the workflows. Moreover, we report on results on the language features typically adopted in workflow specification, with a focus on the concepts that are of particular importance for interactive workflows.


**BIT: Using Bitmap Index to Speed Up NCBI Taxonomy Computing**

_Chuan Hu (Computer Network Information Center, Chinese Academy of Sciences), Jiawei Cai (Computer Network Information Center, Chinese Academy of Sciences), Zihao Zhao (Huawei Technology Company) and Zhihong Shen (Computer Network Information Center, Chinese Academy of Sciences)._ 

Abstract

The National Center for Biotechnology Information (NCBI) Taxonomy is extensively used in biomedical and ecological research. Typical demands include computing the lowest common ancestor, determining descendant relationships, and listing the descendants of a node. However, existing tools often suffer from inefficient runtime performance. To address this challenge, our paper introduces a novel indexing method, BIT, designed specifically for tree-like data. BIT first encodes the tree-like structure into a bit-vector using the Polychotomic encoding algorithm, subsequently storing the bit-vector in a bitmap. By employing parallel bit operations, BIT significantly accelerates the speed of typical computational tasks. Experimental results on public datasets demonstrate that BIT outperforms baseline systems in task execution performance.


## Accepted Short Research Papers

**A Model and Query Language for Multi-modal Hybrid Query**

_Chuan Hu (Computer Network Information Center, Chinese Academy of Sciences), Zihao Zhao (Huawei Technology Company), Along Mao (Computer Network Information Center, Chinese Academy of Sciences) and Zhihong Shen (Computer Network Information Center, Chinese Academy of Sciences)._ 

Abstract

As data grows exponentially, its diversity also increases, including both structured forms and unstructured forms like audio, images, and videos. Advances in AI have improved our ability to analyze unstructured data, leading to the use of multimodal hybrid queries that blend structured and unstructured data. However, database systems struggle due to the lack of adequate data models for multimodal data and languages for these hybrid queries. This paper extends the property graph model to represent multimodal data and their semantic information, introducing essential functions for hybrid graph queries. A high-level graph query language, CypherPlus, is presented, capable of expressing hybrid queries like “Give me the friends of the friends of Mary, who have blond hair and are younger than 30 years old.” A Neo4j-based implementation and experiments over synthetic and real-world datasets demonstrate the approach's plausibility.

**Towards a Temporal Graph Query Language for Durable Patterns**

_Daniel Betsche (Karlsruhe Institute of Technology (KIT)), Klemens Böhm (Karlsruhe Institute of Technology (KIT)), Balduin Katzer (Karlsruhe Institute of Technology (KIT), Karlsruhe University of Applied Sciences (HKA)) and Katrin Schulz (Karlsruhe Institute of Technology (KIT), Karlsruhe University of Applied Sciences (HKA))._ 

Abstract

Dynamic graphs are often the initial data for scientific analyses.
However, existing methods designed for static graphs struggle with efficiency and accuracy when applied dynamically.
One challenge occurs when local interactions in dynamic graphs influence global phenomena.
Practitioners then follow the evolution of relationships between individual elements in local structures.
Such structures are called Durable Graph Patterns or evolving subgraphs.
This work introduces the Durable Graph Pattern Query Language (DPQGL), which allows for user-friendly querying of durable graph patterns on dynamic graphs.
DPGQL is, by design, agnostic to the underlying durable pattern-matching algorithm.
We base our proposed language on the widely used Cypher Query Language.
In our experiments with seven pattern shapes in 24 variations on real-world materials science data, we explore the impact on query runtimes from query complexity and the frequency of graph changes. world, non-IID dataset scenarios, even though they do not approximate the ideal performance of CML.


**Knowledge Graph Enhancement for Improved Natural Language Health Question Answering using Large Language Models**

_Hasan Jamil (University of Idaho) and Joel Oduro-Afriyie (University of Idaho)._ 

Abstract

In this paper we present a method for enhancing Question Answering (QA) systems by iteratively improving Knowledge Graphs (KGs) with a focus on maintaining monotonicity in the enhancement process. We introduce a mathematical framework employing functions $\tau$ and $\phi$, where $\tau$ transforms text $T$ into a KG $K$, and $\phi$ generates an answer from $T$ for a given question. We propose that augmenting $K$ with domain-specific information, denoted as $\Delta^K$, leads to a more accurate approximation of the expected answer, adhering to the principle that each enhancement either maintains or improves answer quality. This concept is formalized as $\phi^{-1}(\phi(T)\cup \Delta^K)$ yielding better results than $\phi^{-1}(\phi(T))$. The paper elaborates on this process with practical examples, demonstrating how KG enhancements, under the constraints of monotonicity, lead to successive improvements in the Question Answering (QA) system.

**Why Do Scientific Workflows Still Break?**

_Nahan Maligeay (Université Paris-Dauphine, PSL Research University - CNRS UMR [7243] LAMSADE), Noémie Bossut (Université Paris-Dauphine, PSL Research University - CNRS UMR [7243] LAMSADE) and Khalid Belhajjame (Université Paris-Dauphine, PSL Research University - CNRS UMR [7243] LAMSADE)._ 

Abstract

Scientific workflows have established themselves as valuable tools for designing, automating, and sharing scientific experiments and analyses, with the aim of promoting reproducibility and reuse. However, early evidence from a decade-old experiment revealed that a significant portion of workflows suffer from decay, making them difficult to rerun or repeat successfully. In this paper, we offer a fresh perspective on this issue, focusing on workflows specified using two popular workflow systems: SnakeMake and NextFlow. Our analysis seeks to address several key questions: Is workflow decay still a prevalent issue? Are the causes of decay similar to those observed in previous generations of workflows, or are new factors at play? What mechanisms and techniques can be employed to mitigate workflow decay? We present an empirical analysis based on an examination of SnakeMake and NextFlow workflows documented in two workflow repositories: WorkflowHub and nf-core.


**WebAssembly serverless join: A Study of its Application**

_Chanattan Sok (Univ Rennes, CNRS, IRISA), Laurent D'Orazio (Univ Rennes, CNRS, IRISA), Reyyan Tekin (Thales Group) and Dimitri Tombroff (Thales Group)._ 

Abstract

Big data’s impact is driving research into efficient solutions for managing growing datasets, with a focus on distributed systems. Recent advancements in query processing, particularly the join operator, have been significant. WebAssembly (Wasm), known for its efficiency, is increasingly adopted. This project aims to evaluate the efficiency of Wasm in serverless environments, addressing challenges posed by serverless architectures and comparing Wasm-based joins against native in performance. We propose Blossom, a Rust-based experimental platform, to give insights into Wasm-based joins. Our initial results reveal trade-offs between Wasm performance and its generality.


**On Vulnerability of Access Control Restrictions to Timing Attacks in a Database Management System.**

_Alexander Rasin (DePaul University), James Herbick (DePaul University), Ben Lenard (Argonne National Laboratory, DePaul University), Nick Scope (DePaul University) and James Wagner (University of New Orleans)._ 

Abstract

Side-channel attacks leverage implementation of algorithms to bypass security and leak restricted data. A timing attack observes differences in runtime in response to varying inputs to learn restricted information. Most prior work has focused on applying timing attacks to cryptoanalysis algorithms; other approaches sought to learn about database content by measuring the time of an operation (e.g., index update or query caching). Our goal is to evaluate the practical risks of leveraging a non-privileged user account to learn about data hidden from the user account by access control.
As with other side-channel attacks, this attack exploits the inherent nature of how queries are executed in a database system.  Internally, the database engine processes the entire database table, even if the user only has access to some of the rows. We present a preliminary investigation of what a regular user can learn about “hidden” data by observing the execution time of their queries over an indexed column in a table. We perform our experiments in a cache-control environment (i.e., clearing database cache between runs) to measure an upper bound for data leakage and privacy risks. Our experiments show that, in a real system, it is difficult to reliably learn about restricted data due to natural operating system (OS) runtime fluctuations and OS-level caching. However, when the access control mechanism itself is relatively costly, a user can not only learn about hidden data but they may closely approximate the number of rows hidden by the access control mechanism.


**VG-Prefetcher Cache: Towards Edge-Based Time Series Data Management Using Visibility Graph Prefetching**

_Akram Bensalem (CNRS, Lab-STICC), Laurent D'Orazio (CNRS, IRISA), Julien Lallet (Nokia Bell Labs France) and Andrea Enrici (Nokia Bell Labs France)._ 

Abstract

The demand for efficient and reliable cloud computing systems is
increasing. However, effectively managing data workloads in edge
cloud systems, especially for connected cars, can be challenging.
To address this issue, we have developed a new cache management
technique named VG-Prefetcher Cache that uses visibility graphs to
handle time series data more effectively. Our approach involves predicting future data and prefetching it into the cache, which reduces
retrieval time and improves system performance. VG-Prefetcher
Cache presents a promising approach for overcoming challenges in
managing data workloads, thus paving the way for a more efficient
and reliable cloud computing system.


## Accepted Demonstration Paper

**Performance-cost trade-offs in service orchestration for edge computing**

_Daniel Balouek (Inria)._ 

Abstract

Low latencies connections and decentralized servers are currently showcasing a new potential for distributed computing. By moving away from traditional centralized cloud models and toward edge computing, which allows for more autonomy and decision-making at the network's edge, almost any physical thing can be turned into an Internet of Things (IoT) device that can elaborate on data it senses from its environment. In this context, service management and adaptation routines in a highly dynamic and geographically distributed federation depends on a large number of factors ranging from performance to cost and the fluctuation of the data input size and quality.
This paper presents mechanisms for monitoring resources at the edge in real-time, orchestrating service provisioning, performing data-driven decisions on behalf of applications, adapting service locations, and coordinating sensing tasks. The demonstration focuses on autoscaling of containers, service placement and distributed sensing, while considering utility metrics to help achieve a fluid workload in Kubernetes clusters.



## Accepted Poster Presentation

**Efficient Streaming Analysis of High-Resolution Plasma Transport**

_Junmin Gu (Lawrence Berkeley National Laboratory), Paul Lin (Lawrence Berkeley National Laboratory), Kesheng Wu (Lawrence Berkeley National Laboratory), Seung-Hoe Ku (Princeton Plasma Physics Laboratory), C.S Chang (Princeton Plasma Physics Laboratory), Robert Hager (Princeton Plasma Physics Laboratory), Aaron Scheinberg (Jubilee Development) and Jong Youl Choi (choij@ornl.gov)._

**Enhancing Observatories with Fog Computing**

_Ammar Kazem (Univ. Rennes, Inria, CNRS, IRISA), Guillaume Pierre (Univ. Rennes, Inria, CNRS, IRISA) and Laurent Longuevergne (Geosciences Rennes–UMR 6118, Univ. Rennes, CNRS)._

**Towards Optimizing Data Movement in the Computing Continuum Workflow**

_Radita Liem (RWTH Aachen University) and Shadi Ibrahim (Inria, Univ. Rennes, CNRS, IRISA)._

**On The Energy Footprint of Erasure Codes in Ceph**

_Marc Tranzer (Inria, Univ. Rennes, CNRS, IRISA) and Shadi Ibrahim (Inria, Univ. Rennes, CNRS, IRISA)._

**Quantifying the Performance of Erasure Codes in P2P Storage Systems**

_Mohammad Rizk (Inria, Univ.  Rennes, CNRS, IRISA, Rennes, France), Shadi Ibrahim (Inria, Univ.  Rennes, CNRS, IRISA, Rennes, France) and Thomas Lambert (Universite   de Lorraine, Inria, LORIA, Nancy, France)._

**Privacy-Preserving Distributed Spectral Centrality Measures based on Fully Homomorphic Encryption**

_Claire Guichemerre (Univ Rennes, CNRS, IRISA), Tristan Allard (Univ Rennes, CNRS, IRISA), Sofiane Azogagh (Univ Québec à Montréal), Sébastien Gambs (Univ Québec à Montréal), Marc-Olivier Killijian (Univ Québec à Montréal) and Amr El Abbadi (Univ California Santa Barbara)._

_Accepted Short Research Papers will also participate in the Poster Session._
