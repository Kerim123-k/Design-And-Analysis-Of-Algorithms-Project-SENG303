# Design-And-Analysis-Of-Algorithms-Project-SENG303
# Literature Review: Louvain Algorithm for Community Detection

## Overview

This project presents a structured literature review of the Louvain algorithm for community detection in complex networks.

The review is based on the systematic analysis of 80 peer-reviewed research papers published between 2008 (the original Louvain paper) and 2025.

The goal of the study is to understand how the Louvain algorithm has evolved, how it performs in different contexts, and how it compares to modern community detection methods.

---

## Research Questions

The review is organized around three main research questions:

RQ1 – Scalability and Performance  
How efficient is the Louvain algorithm on large-scale networks, and how have parallel and distributed variants improved performance?

RQ2 – Community Quality and Resolution Issues  
How do Louvain-based methods address modularity resolution limits, partition instability, and overlapping community detection?

RQ3 – Comparisons and Applications  
How does Louvain compare to alternative methods (e.g., Leiden, GNN-based models), and how is it used in real-world applications?

---

## Methodology

Databases used:
- Google Scholar
- IEEE Xplore Digital Library

Search phrase:
"Community detection using the Louvain algorithm"

Selection Criteria:
- Peer-reviewed journal and conference papers
- Direct use, modification, or evaluation of Louvain
- English language
- Published from 2008 onward

Final corpus:
80 research papers

Each paper was categorized by:
- Contribution type (variant, application, theoretical analysis)
- Network type (static, dynamic, weighted, multilayer)
- Focus area (scalability, quality, comparison, application)
- Evaluation metrics (modularity, NMI, ARI, runtime, memory)

---

## Main Literature Themes

### 1. Scalable and Parallel Louvain Variants

Research shows that Louvain is inherently scalable but can be improved through:

- Heuristic acceleration
- Clique-based optimizations
- GPU implementations
- Distributed computing (Hadoop, Spark)
- Incremental updates for evolving graphs

Common metrics:
- Modularity
- Runtime
- Speedup ratio
- Memory usage

---

### 2. Community Quality and Resolution Improvements

Key improvements focus on:

- Multi-resolution modularity
- Edge reweighting techniques
- CPM-based objective functions
- Overlapping and fuzzy community extensions
- Multi-objective optimization

Important findings:
- Higher modularity does not always mean better ground-truth alignment.
- External metrics like NMI and ARI are crucial.
- Partition stability is a major concern.

---

### 3. Dynamic and Temporal Extensions

Instead of re-running Louvain for every snapshot:

- Incremental Louvain updates local changes
- Multilayer modularity models enforce temporal smoothness
- Game-theoretic and adaptive models improve dynamic tracking

Trade-off:
Temporal smoothness vs sensitivity to sudden structural change.

---

### 4. Domain Applications

Louvain is widely applied in:

- Social media influencer detection
- Recommendation systems
- Power grid analysis
- Water distribution networks
- Fraud detection
- Blockchain security
- Speaker diarization
- Graph neural network pipelines

In many applications, Louvain is used as:
- A baseline algorithm
- A structural preprocessing step
- A feature extraction component

---

## Case Studies Included

1. Distributed Community Detection in Web-Scale Networks  
   - Core-group extraction
   - Hadoop / MapReduce implementation
   - Linear runtime scalability

2. Louvain vs Leiden in Influencer Detection  
   - Leiden achieved higher modularity and lower runtime
   - Fewer but more consolidated communities

3. Weighted Louvain  
   - Edge weights improve modularity
   - Better quality than standard Louvain
   - Leiden often faster but slightly lower modularity

---

## Key Insights

- Louvain remains a strong benchmark algorithm.
- Performance can be improved with parallelization.
- Modularity alone is insufficient to measure quality.
- Resolution limits remain a known challenge.
- Stability and robustness require ensemble or consensus approaches.
- Louvain continues to be used even alongside modern GNN methods.

---

## Identified Research Gaps

- Few methods jointly handle dynamic + overlapping + attributed networks.
- Evaluation practices lack standardization.
- Robustness testing is often limited.
- Multi-objective and learning-based hybrids are promising future directions.

---

## Proposed Computational Study

Planned experimental comparison:

Baseline:
- Original Louvain

Variant:
- Multi-resolution Louvain OR Leiden

Datasets:
- Synthetic LFR benchmark
- Real-world social network

Metrics:
- NMI
- ARI
- Modularity
- Runtime

Goal:
Validate literature-reported trade-offs between quality and performance.

---

## Conclusion

The Louvain algorithm has evolved from a single modularity optimization method into a broad family of scalable, adaptable, and application-integrated approaches.

While newer algorithms (e.g., Leiden, GNN-based methods) may outperform Louvain in specific tasks, Louvain remains:

- Computationally efficient
- Structurally interpretable
- Widely adopted as a baseline
- Highly extensible

Its simplicity and scalability ensure it remains a foundational method in community detection research.

---

## Team Contributions

Kerim Hariri – Project integration and final editing  
Mohamad Attia Eid – Literature organization and citations  
Elnur Aliyev – Technical validation and diagrams  
Zaid Hardan – Methodology and comparative analysis  

Each member reviewed and summarized 20 research papers.

---

## Full Report

The complete literature review report is available in this repository as a PDF file.
The repository also includes the excel sheet that was used for the project and the presentation we used inside our class.
