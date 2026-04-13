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

Automated quality assurance for multi-artifact programming exercises is an important component of scalable computer science education. Existing systems that use large language models (LLMs) to detect inconsistencies between exercise components demonstrate fundamental feasibility, but suffer from significant limitations in detection precision, leading to high rates of false positives. The current approach does not explicitly model the relationships between exercise components, such as problem statement, code templates, sample solutions and tests repositories.

We extend the existing system by establishing an on-demand benchmarking workflow and expanding the dataset with 16 real university exercises to enable comparable, reproducible evaluation. To reduce false positives, we add a language-aware context filter and a verification checker that re-evaluates detected issues before reporting. To address the structural limitation directly, we model semantic and structural relationships between exercise artifacts via a knowledge-graph-based context representation and integrate it into the LLM-based consistency check pipeline. Together, these contributions aim to deliver a more reliable and sustainable system for ensuring the quality of education.

We defined the following objectives to achieve described goals:
1. Establish an On-Demand Benchmarking Workflow.
2. Extend Consistency Check Dataset.
3. Improve Consistency Issues Detection.
4. Enhance Context Representation.

[Mikhail Khinevich Thesis Proposal](proposal.pdf)
