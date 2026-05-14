---
title: "Keynote & Invited Talks"
weight: 4
theme: "damon-dark"
---

# Keynote & Invited Talks

## Keynote Talk
### Accelerating Queries at CoddSpeed: Hardware Coprocessors on the Road to Production
<h4 style="text-align: center;">Nico Bruno & Matteo Interlandi, Microsoft Jim Gray Labs</h4>

{{< image-row gap="5">}}
![Portrait of Nico Bruno](/img/nico_bruno.jpg)
![Portrait of Matteo Interlandi](/img/matteo_interlandi.jpg)
{{< /image-row >}}

**Abstract**:
Modern cloud platforms expose a growing portfolio of specialized hardware — GPUs, FPGAs, DPUs, AI accelerators, etc. — that have the potential to bring substantial speedups to analytical query processing. Ideally, a single generic coprocessor design would let us capture this potential inside a mature commercial database engine: in practice, this is remarkably hard. The real challenges are rarely the kernels themselves: type systems, ANSI semantics, data-layout encodings, hardware availability, and the engineering-process discipline of a production codebase that thousands of customers depend on.

This talk is about CoddSpeed, our effort within the Microsoft Fabric Data Warehouse to build a general substrate for hardware-accelerated query execution that can host different coprocessors over time. We frame the recurring problems any such integration must solve, the architectural decisions we have converged on, and the real-world production surprises that inevitably surface when moving beyond controlled workloads. We ground the talk in our experience with TQP (Tensor Query Processor), a GPU coprocessor whose journey from a research prototype into a system built by 60+ engineers offers a candid case study in what it takes to move accelerator research from the lab to a shipping product. We close with reflections on trust, thoroughness, and concrete strategies for de-risking accelerator research on the road to production.

<details>
  <summary>About the Speakers</summary>

**Nicolas Bruno** is Partner Director of Research in the Microsoft Gray Systems Lab. He received his PhD from Columbia University in 2003 and has held leading roles in query optimization across Microsoft, Google, AWS, and Snowflake, including work on Cosmos/Scope, Spanner, and Azure Data. Since 2023, he has been back at Microsoft Research, bridging research and development in data systems.

**Matteo Interlandi** is a Principal Research Scientist in the Microsoft Gray Systems Lab, working at the intersection of machine learning and database systems. His work has received recognition at SIGMOD and VLDB, including an honorable mention at SIGMOD 2021, a best demo award at VLDB 2022, and selection for the 'Best of VLDB 2016'. Before joining Microsoft, he held research positions at UCLA, the Qatar Computing Research Institute, and the Institute for Human and Machine Cognition. He received his PhD in Computer Science from the University of Modena and Reggio Emilia.
</details>

--- 

## Fresh Thinking Talk 1
### Towards a Programmable Data-Centric AI Stack for Processing-In-Memory Architectures
<h4 style="text-align: center;">Christina Giannoula, Max Planck Institute Software Systems</h4>

![Portrait of Christina Giannoula](/img/christina_giannoula.jpg)

**Abstract**:
Processing-in-Memory (PIM) architectures integrate compute cores close to or within memory arrays, emerging as a promising paradigm to accelerate memory-intensive kernels in modern Machine Learning (ML) models. While ML models contain both compute-intensive and memory-intensive kernels, the latter are often bottlenecked by limited memory bandwidth in conventional CPU and GPU systems. Industry manufacturers and researchers have therefore extensively explored PIM devices and their integration with host CPU/GPU systems to enable efficient end-to-end ML model execution. However, fully leveraging PIM's benefits for ML applications requires a system software stack that is data-centric and programmable.

This talk explores how specialized libraries, system software, and compilers can unlock the potential of PIM architectures for machine learning workloads. First, I will present PyGim, a novel Graph Neural Network (GNN) library designed specifically for PIM systems, which optimizes memory-intensive GNN kernels through intelligent parallelization strategies. Second, I will introduce DCC, the first data-centric ML compiler for PIM architectures, supporting diverse ML kernels across heterogeneous PIM backends. I will conclude by illustrating that rethinking various stack components to be data-centric and programmable can be the key enabler for the wide adoption of PIM architectures in modern ML systems.

<details>
  <summary>About the Speaker</summary>
Christina Giannoula is a Tenure-Track Faculty member at the Max Planck Institute for Software Systems (MPI-SWS), where she leads the SPIN research group. Her research lies at the intersection of computer architecture, computer systems, and sustainable computing for emerging AI models. Her current research focuses on rethinking system components across the entire stack, including algorithms, compilers, runtime systems, programming frameworks, and hardware engines, to be data-centric and application-aware. She has authored numerous papers published at premier computer architecture and systems venues, including ISCA, HPCA, MICRO, ASPLOS, EuroSys, and MLSys. Her contributions to the field have been recognized through several prestigious awards and fellowships, among them the 2024 MLSys Rising Star Award, the 2024 EECS Rising Star Award, Postdoctoral Awards from the Vector Institute for Artificial Intelligence, an Outstanding Paper Honorable Mention at MLSys 2025, and the 2022 Iakovos Gurounian Award for the doctoral thesis of highest industrial impact. She holds a Ph.D. from the National Technical University of Athens (NTUA) and completed her postdoctoral research at the University of Toronto.
</details>

## Fresh Thinking Talk 2
### Query Execution Beyond the CPU
<h4 style="text-align: center;">Kwanghyun Park, Yonsei University</h4>

![Portrait of Kwanghyun Park](/img/kwanghyun_park.jpg)

**Abstract**:
Modern DBMSs have long been designed around a CPU-centric assumption: query operators execute on the processor, while memory and storage passively provide data. This abstraction has been remarkably successful, but it is increasingly strained by modern workloads and hardware trends. Emerging technologies such as persistent memory, near-data processing, computational storage, heterogeneous accelerators, and CXL-based memory fabrics are changing where computation can and should occur. At the same time, AI-driven workloads such as vector search and retrieval pipelines amplify the cost of data movement, making centralized execution less attractive.

In this talk, I discuss how query execution is moving beyond the CPU and becoming distributed across memory, storage, and interconnect fabrics. I will further explore how this shift challenges traditional DBMS assumptions and motivates new abstractions for execution placement, data movement optimization, topology-aware scheduling, and memory-centric query
processing.

<details>
  <summary>About the Speaker</summary>
Kwanghyun Park is an Assistant Professor in the Department of Computer Science at Yonsei University, where he leads the BDAI (Big Data & AI) Lab. His research focuses on next-generation data systems spanning systems for machine learning, hardware-aware database systems, vector search and AI data infrastructure, and hardware–software co-design for emerging memory and storage architectures. His recent work explores memory-centric query processing, near-data processing, heterogeneous execution, and CXL-based AI data systems. Before joining Yonsei University in 2023, he was a Senior Research Engineer at Microsoft Gray Systems Lab, where he worked on large-scale data and ML systems for cloud platforms and enterprise workloads. He received his Ph.D. and M.Sc. in Computer Science from the University of Wisconsin–Madison.
</details>

--- 

## Sponsor Talk

### Transparent Huge Pages to the Rescue for In-Memory Data Processing?
<h4 style="text-align: center;">Norman May, SAP</h4>

![Portrait of Norman May](/img/norman_may.jpg)

**Abstract**:
SAP HANA is known for its high-performance in-memory processing performance, especially for mixed OLAP and OLTP workloads. Hence, it may come as a surprise that SAP HANA did not support transparent huge pages (THP) when using them promises better performance and scalability.  In the talk I will present a brief history on our journey towards supporting THP and share some challenges to overcome along the way. 

<details>
  <summary>About the Speaker</summary>
Norman May is a graduate of the University of Mannheim, Germany, and the University of Waterloo, Canada, where he studied Business Administration and Computer Science. He received his doctoral degree from the University of Mannheim, focusing on query optimization and query execution for analytical and XML queries.
After joining SAP SE in 2007, he worked as a researcher at SAP Research and later at the SAP HANA Campus, collaborating with several students and research groups. His work has been published in leading international database conferences and journals. He has also served the database community as a reviewer and chair for major database conferences and workshops, including DAMON.
Since 2010, he has contributed to the development of the SAP HANA database in roles of increasing responsibility, ultimately becoming a chief architect, focusing on query processing, modern hardware, and multi-tenancy.
</details>
