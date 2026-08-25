# Dissertation Supplementary Materials

This repository provides supplementary material for a doctoral dissertation on structural quality assessment and infrastructure recommendation for microservice-based systems. The research connects three concerns that are often studied separately: detection of microservice design patterns and antipatterns, benchmark-based evaluation of detection methods, and recommendation of a suitable Infrastructure-as-a-Service (IaaS) offering for deploying a selected microservice.

## Research workflow

The workflow begins with a dataset of microservice-based systems. Static-analysis artifacts—including service dependencies, annotations, imports, configuration files, and system structure—are used to detect architectural patterns and antipatterns. The resulting evidence supports a structural quality assessment of the candidate microservices. Detection methods are evaluated and compared through an automated benchmark, after which the selected high-quality microservices are passed to the infrastructure-recommendation stage.

![Dissertation workflow: from microservice pattern and antipattern detection to IaaS recommendation](docs/dissertation-workflow-en.png)

The five stages shown in the figure are:

1. **Microservice systems.** A collection of microservice-based systems provides the research input and the architectural artifacts required for analysis.
2. **Pattern and antipattern detection.** Supported design patterns and antipatterns are identified, and the microservices are reviewed and classified according to their structural design quality.
3. **Benchmark-based evaluation.** Competing detection methods are assessed using accuracy, recall, reliability, coverage, and scalability. The benchmark validates, ranks, and compares the methods so that a suitable method can be selected for dependable pattern and antipattern detection.
4. **Infrastructure recommendation.** Microservices with equivalent business functionality may differ in non-functional characteristics such as cost, reliability, availability, and efficiency. Fuzzy C-Means (FCM) clustering reduces the cloud-provider search space, while customer preferences are processed by IANFRA to score candidate services and recommend a suitable IaaS option.
5. **Final output.** A microservice with appropriate design quality is deployed on a suitable infrastructure service, with the objective of improving performance, cost suitability, quality, and user satisfaction.

## Supplementary appendix files

The dissertation refers to the following three supplementary files. They are separated by purpose so that each appendix can be cited, reviewed, or included independently.

| File | Purpose |
| --- | --- |
| [`appendix-a-patterns-antipatterns.pdf`](appendices/appendix-a-patterns-antipatterns.pdf) | Defines the microservice design patterns and antipatterns examined in the dissertation, explains their architectural intent or quality risk, and states why they can be detected through static analysis. |
| [`appendix-b-pattern-mining-methods.pdf`](appendices/appendix-b-pattern-mining-methods.pdf) | Documents the two pattern-mining procedures: the Support Vector Machine (SVM) method and the graph-based method using node labeling, edge filtering, Dual Simulation, and global-constraint validation. |
| [`appendix-c-svm-feature-vector.pdf`](appendices/appendix-c-svm-feature-vector.pdf) | Gives the detailed definition and initialization of the 30-element SVM feature vector, including Master, Worker, and Client roles and the worked API Gateway subgraph example. |

