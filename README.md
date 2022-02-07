# Comp790-166: Computational Biology (Spring 2022) 

## Details

Instructor: Natalie Stanley

Email: natalies@cs.unc.edu

**Note : Please send me an email if you enrolled late and did not recieve the welcome email!**

Time and Place: Monday/Wednesday 9:30am-10:45am in Sitterson 115 (SN0115) and on Zoom. This course will be offered as a hybrid course. I will be present in SN0115 for each class meeting and also be on zoom and recording the lecture. Please watch your emails for a zoom link. 

 Info and Attributes: This is a 3-credit full-semester course and fulfills the 'Applications' category for CS students. It is a lecture-style class (I will teach the lectures) and includes two homework assignments and a course project. Please make sure you selected the 3-credit option when you enrolled. 

Office Hours: Monday 10:45-noon or by appointment 

## Description
Modern, high-throughput assays allow us to efficiently profile a variety of biological processes to gain a systems-level understanding of health and disease. Recent technologies and experimental assays generate an abundance of detailed information that needs to be extracted, summarized, and interpreted. In this course we will discuss the methodology used to extract signal from (e.g. process, engineer features from, combine, etc.) data generated by some of the most cutting-edge experimental paradigms, such as single-cell assays and imaging. We will go into detail about the methods and theory underlying bioinformatics algorithms, originating from numerical linear algebra, graph-signal processing, and machine learning. While computational biology is a very broad field, we will focus here on applications in single-cell biology (CyTOF, single-cell RNA sequencing), multiomics/multi-modal analysis, systems immunology, and benchmarking. For each class of algorithms introduced for some task on biological data, we will also go over necessary theory and mathematical intuition. The course covers the foundations for biomedical data science and does not assume any biological knowledge.

## Prerequistes
Students should be strong in programming in Python or Julia or R, and be comfortable with linear algebra and basic probability. **I do not assume any prior biological knowledge. Any relevant concepts will be introduced**. Please feel free to talk to me about any of these prerequistes. 

## Course Structure
This course will be mostly lecture-based with two homework assignments and a course project. I will provide ideas for several publicly available biological datasets and open problems for you to work on for these projects. Overall, the project is intended to give you an opportunity to implement/apply methodology discussed in the papers that we will discuss together. The final project writeup will also give you practice writing up results and communicating ideas. You are welcome to work on teams for this project.

Students will also pick any two days during the semester to answer a set of reading questions about one of the assigned papers. 

# Topics and Tentative Schedule. 

This is the preliminary set of topics. 


| Date | Topic | Reading | Notes | Code |
|------|-------|---------|-------|------|
|Monday January 10, 2022 | Intro, Bioinformatics vs Computational Biology| [[Systems Immunology, Just Getting Started](https://www.nature.com/articles/ni.3768)], [[Grand Challenges in Single-Cell Data Science](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-020-1926-6)] | [[Lecture 1 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture1_public.pdf)] | 
|Wednesday January 12, 2022| Linear Algebra Review, Matrix Rank, Building Graphs from Data, Graph Laplacian, Graph Diffusion | [[SLMP. pages 10-22](https://arxiv.org/abs/2004.07984)], [[Data Matrices + Low Rank](https://arxiv.org/abs/1705.07474)], [[Random Projection Trees](https://cseweb.ucsd.edu/~dasgupta/papers/rptree-stoc.pdf)],[[LargeVis](https://arxiv.org/abs/1602.00370)] | [[Lecture 2 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture2_public.pdf)] | [[graph tools for python](https://github.com/KrishnaswamyLab/graphtools)] |
|Monday January 17, 2022| **No class for MLK Day, and no regular office hours today. Please email me to set up a meeting for anything urgent.** |
|Wednesday January 19, 2022|Overflow from last time introducing the diffusion point of view of graph laplacian ; building graphs from data; Graph Partitioning Fundamentals| [[Module Detection Benchmarking in Biological Data](https://www.nature.com/articles/s41592-019-0509-5)], [[BigClam](https://cs.stanford.edu/people/jure/pubs/bigclam-wsdm13.pdf)], [[SBM for single-cell](https://link.springer.com/article/10.1186/s12859-021-04489-7)] | [[Lecture 3 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture3_public.pdf)] | [[LargeVis](https://github.com/lferry007/LargeVis)]  |
|Monday January 24, 2022| Graph Partitioning (Modularity-Based {Louvain, Leiden}; Finding disease-relevant modules from protein-protein and/or gene-gene interactions networks | [[Fast Unfolding of Communities in Large Networks](https://arxiv.org/abs/0803.0476)] | [[Lecture 4 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture4_public.pdf)]  | [[SNAP](https://snap.stanford.edu/)], [[Louvain](https://github.com/vtraag/louvain-igraph)], [[Leiden](https://github.com/vtraag/leidenalg)], [[graph-tool (SBM)](https://graph-tool.skewed.de/)], [[pyGSP](https://pygsp.readthedocs.io/en/stable/)] |
|Wednesday January 26| Finish probabilistic graph partitioning {SBM, Affiliation Model}); Graph Embeddings with node2vec (such as node2vec);  Single-Cell Day 1 : Intro to Single-Cell Profiling and Data Structures  | [[Node2Vec](https://dl.acm.org/doi/pdf/10.1145/2939672.2939754?casa_token=vQTboPUL6qIAAAAA:XQsAUtXd4MyWfj1ClUBw8FKhuPbpqO-aE2d7EDs5iX9-jJZP9BuxDbKUjg3CM69YKHALjCAKJtJx)], [[Representation Learning on Graphs](https://arxiv.org/abs/1709.05584)], [[Review: Graph Embedding in Comp Bio](https://www.frontiersin.org/articles/10.3389/fgene.2019.00381/full)], [[Vicus](https://journals.plos.org/ploscompbiol/article/authors?id=10.1371/journal.pcbi.1005621)] , **omitted for lack of time, but will come back to later (Graph Signal Processing (GSP) Basics**[[Intro to Graph Signal Processing in Machine Learning](https://web.media.mit.edu/~xdong/paper/spm20.pdf)] | [[Lecture 5 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture5_public.pdf)] | [[node2vec](https://github.com/aditya-grover/node2vec)] | 
|Monday January 31| Single Cell Day 1: Intro to Single-Cell {Data Structure, Technologies, Pre-Processing}, Automating Gating and Cell-Population Discovery in Single Cell Data| [[Spade](https://www.nature.com/articles/nbt.1991)], [[Single-Cells, Many Features](https://www.sciencedirect.com/science/article/pii/S009286741630410X)] | [[Lecture 6 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture6_public.pdf)]  | [[FCS file tutorial](https://github.com/stanleyn/fcs_tutorial)], [[Spade](https://github.com/nolanlab/spade)]   |
|Wednesday February 2| Graph-based automated gating, imputation in single-cell data|  [[phenograph](https://www.sciencedirect.com/science/article/pii/S0092867415006376)] | [[Lecture 7 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture7_public.pdf)] | [[phenograph](https://github.com/JinmiaoChenLab/Rphenograph)],  [[FastPG](https://github.com/sararselitsky/FastPG)] |
|Monday February 7| Imputation for single-cell data, Branch Preserving Visualization for Single-Cell Data| [[MAGIC](https://www.biorxiv.org/content/10.1101/111591v1)],[[PHATE](https://www.nature.com/articles/s41587-019-0336-3)],  | | [[Lecture 8 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture8_public.pdf)] |  [[MAGIC](https://github.com/KrishnaswamyLab/MAGIC)],[[Phate](https://github.com/KrishnaswamyLab/PHATE)]  | 
|Wednesday February 9| Data Augmentation for Single Cell Identifying prototypical cells of a particular experimental condition with graph signal processing| [[SUGAR](https://arxiv.org/abs/1802.04927)],[[MELD](https://www.biorxiv.org/content/10.1101/532846v4)], [[Graph Signal Processing Review Article](https://web.media.mit.edu/~xdong/paper/spm20.pdf)] | | [[sugar](https://github.com/stanleyjs/sugar)], [[MELD](https://github.com/KrishnaswamyLab/MELD)] |
|Week 6-1| Graph-based differential cell-population abundance analysis and differential abundance testing with spatial FDR, Contrastive PCA|
|Week 6-2| Combining Multiple Single-Cell Datasets|
|Week 7-1| Combinding multiple panels (e.g. single-cell data with different measured features), Pseudotime and trajectory inference|
|Week 7-1| Project Proposal Presentations Day 1|
|Week 7-2| Project Proposal Presentations Day 2|
|Week 8-1| Combining biological data from multiple modalities using Grassmann Embeddding|
|Week 8-1| Longitudinal multi-modal integration and neuroscience application|
|Week 9-1| Convex Optimization and ADMM|
|Week 10-1| 'Multiomics Factor Analysis' for integrating multiple modalities and multiple single-cell modalities|
|Week 10-2| Integrating Graphs with Multiple Relational Definitions (e.g. same nodes, different edges), Intro to Network Alignment|
|Week 11-1| Refining Graph Alignments and Graph Summarization|
|Week 12-2| Harmonic Alignment for integrating multiple single-cell datasets, Graph Neural Networks vs. Label Propagation|
|Week 13-1| Graph Neural Networks to integrate spatial information with genomic data|
|Week 13-2| Imagining Proteomics and Genomics and Spatial Regularization|
|Week 14-1| Computational Neuroscience and Time-Varying Analysis of Brain Connectivity| 
|Week 15-1| Sketching single-cell datasets day 1
|Week 15-2| Sketching single-cell datasets day 2
|Week 16-1| Technical writing in comp bio, opportunities for graph learning in biology, summary of topics covered|
|Week 16-2| Project Presentations Day 1
|Week 17-1| Project Presentations Day 2
|Week 17-2| Project Presentations Day 3
|Final Exam Day| Final Project Writeups Due

# Key Dates

* **Homework 1 Due:** February 23 (assigned by February 9)
* **Project Proposal Due:** March 9
* **Homework 2 Due:** April 20
* **Final Project Due:** Final Exam Day 

# Homework, Project, Reading, Grading, Etc

## Homework
There will be two homework assignments to practice implementing particular concepts. Often, things can become a bit easier to understand and use when they are implemented by you. I will provide code and hints in Python, but will be happy to read/run code written in Python, R, Julia, or Matlab. Please submit your homework writeup as a PDF. 

## Background Resources
Most of what we discuss in class will come from papers. However, I suggest the following textbooks as background references. Conveniently, they are also available for free.

* [PRML] Pattern Recognition and Machine Learning-- Chris Bishop [[Link](http://users.isr.ist.utl.pt/~wurmd/Livros/school/Bishop%20-%20Pattern%20Recognition%20And%20Machine%20Learning%20-%20Springer%20%202006.pdf)]

* [SLMP] Spectral Learning on Matrices and Tensors -- Majid Janzamin et al. [[Link](https://arxiv.org/abs/2004.07984)]

* The Matrix Cookbook [[Link](https://www.math.uwaterloo.ca/~hwolkowi/matrixcookbook.pdf)]

* [PML] Probabilistic Machine Learning: An Introduction. -- Kevin Murphy [[Link](https://probml.github.io/pml-book/book1.html)]

* [GRL] Graph Representation Learning -- William Hamilton [[Link](https://www.cs.mcgill.ca/~wlh/grl_book/)

* My favorite general linear Algebra Resource: Matrix Computational by Golub and Van Loan


## Readings
Each student much choose two class meetings to answer reading questions for one of the discussed papers. Please answer the following questions and send the responses in PDF format to me by the beginning of our class meeting. 

### Reading Questions

**Please choose 2 papers over the course of the semester to do this for, and turn them in before our class meeting 9:30 am to natalies+comp790@cs.unc.edu**. 

1) Please explain in 2 sentences or less what the problem being solved is.

2) What were the main contributions of the authors in this work? (You can answer in a few bullet points). 

3) Please describe 1-2 computational experiments that the authors implemented to test their method.

4) Were the authors the first to attempt this particular problem? If not, did they compare their results to other baselines? Do you think that their evaluation was objective?

5) Do you think that the authors provided enough evidence for why their developed method is an important contribution? If yes, please describe their reasoning here. If you do not think they adequately justified why they worked on this particular problem, please describe your thoughts on that here. 

6) What is one follow-up idea or extension from this work? 

## Final Project
I will provide you with several examples of publicly available biological datasets and problems (https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Datasets.md). Half-way through the semester, you will submit your project proposal and present your idea to the class.  The proposal will be a short document describing 1) The problem 2) A background on other people's attempts to solve this problem and 3) A background on your idea of a solution and 4) the data you will use to test your method. At the end of the semester you will write a short paper explaining your method and results and present your results.

## Grading
 Grading will be based on the following

1) Reading Questions : 15% -- sufficiently 2 completed during the semester
2) Homework 1: 20%
3) Homework 2: 20%
4) Project Proposal : 10%
5) Project final writeup: 30%
6) Class Participation and Attendance : 5%

## Lateness Policy

I understand if things come up. If you need more time on your homework or project proposal, you are welcome to talk to me about it. However, if you simply turn in your homework late without any prior notice, I will deduct 10% of the points per day. There will be no late submissions of the course project permitted. 

## Mask Usage

I don't anticipate any problems with this, but if you do intent to join the class in-person, please make sure to wear a face mask covering your nose and mouth. 

## Accessibility Statement
The University of North Carolina at Chapel Hill facilitates the implementation of reasonable accommodations, including resources and services, for students with disabilities, chronic medical conditions, a temporary disability or pregnancy complications resulting in barriers to fully accessing University courses, programs and activities.
Accommodations are determined through the Office of Accessibility Resources and Service (ARS) for individuals with documented qualifying disabilities in accordance with applicable state and federal laws. See the ARS Website for contact information: https://ars.unc.edu or email ars@unc.edu.

(source: https://ars.unc.edu/faculty-staff/syllabus-statement)

## Diversity Statement
I value the perspectives of individuals from all backgrounds reflecting the diversity of our students. I broadly define diversity to include race, gender identity, national origin, ethnicity, religion, social class, age, sexual orientation, political background, and physical and learning ability. I strive to make this classroom an inclusive space for all students. Please let me know if there is anything I can do to improve, I appreciate suggestions.


