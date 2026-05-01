![Technical University of Munich](tum.png)

<div align="center">

# Bachelor’s Thesis in Information Systems

## AI-Driven Workflow for Inconsistency Remediation in Programming Exercises

### School of Computation, Information and Technology

### -- Informatics --
Author: Mikhail Khinevich

Supervisor: Prof. Dr. Stephan Krusche
</div>


## Abstract

The Technical University of Munich developed Artemis, an open-source learning management system that hosts multi-artifact programming exercises. Each exercise consists of four interconnected artifacts — problem statement, template, solution and test repositories — that instructors and teaching assistants collaboratively create and maintain. Inconsistencies between these artifacts arise when an instructor modifies one artifact but overlooks the corresponding changes in dependent ones, producing mismatched method names or conflicting type declarations. The Hyperion consistency check within Artemis uses large language models (LLMs) to detect these inconsistencies, but suffers from low precision: the baseline produces nearly one false positive for every two correct detections, forcing instructors to manually verify each reported issue.

This thesis addresses the precision bottleneck and the limitations of the existing detection system through three contributions: (1) It establishes a reproducible benchmarking workflow that connects Artemis with PECV-bench, an evaluation framework for consistency detection, enabling systematic comparison of detection approaches under identical conditions. (2) It extends the evaluation dataset from three Java exercises with 91 variants to 16 exercises with 325 variants across six university courses and multiple programming languages, including Python, C, Assembler, SQL, and Swift. (3) It improves detection precision by introducing a language-aware context filter that removes irrelevant files before analysis and a verification checker that re-evaluates each detected issue to filter false positives.

The verification checker improves precision from 0.531 to 0.819 while maintaining recall at 0.767, raising the F1 score from 0.633 to 0.793 on the extended dataset. Instructors benefit from a lower false positive rate, which reduces manual review and increases the reliability of the automated analysis. The approach relies on closed-source LLM APIs, which introduce non-determinism and limit reproducibility. Abstract Syntax Trees, Knowledge Graphs, and Graph-based Retrieval-Augmented Generation represent the primary direction for future work targeting the remaining false positives.

We defined the following objectives to achieve described goals:
1. Establish an On-Demand Benchmarking Workflow.
2. Extend Consistency Check Dataset.
3. Improve Consistency Issues Detection.
4. Enhance Context Representation (Future Work).

[Mikhail Khinevich Thesis Proposal](proposal.pdf)
