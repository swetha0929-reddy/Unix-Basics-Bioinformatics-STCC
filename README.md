# STCC – Unix Basics for Bioinformatics


Course Documentation and Hands-on Practice  
**Student:** Thamanna Swetha Reddy  
**Institution:** Bversity School of Bioscience  


---


## Overview


This repository documents Unix command-line concepts and tools learned during the **Short-Term Course on Unix (STCC)**, with a strong focus on **bioinformatics and genomic data analysis workflows**.


The project demonstrates how Unix utilities are used for:
- File system navigation
- Streaming and inspecting large biological files
- Text processing and pattern matching
- Working with FASTA files
- Version control using Git and GitHub


This README is written as a **clear, reusable guide**, not just a list of commands, following good bioinformatics documentation practices.


---


## Learning Objectives


By completing this mini project, I demonstrate the ability to:


- Navigate Unix/Linux file systems confidently
- Create, modify, and manage files and directories
- Use Unix utilities to inspect and analyze biological data
- Work with FASTA sequence files
- Use Git and GitHub for version control and reproducible research


---


## Tools & Environment


- Operating System: Ubuntu (WSL)
- Shell: Bash
- Text Editor: nano
- Version Control: Git & GitHub


---


## Unix Basics Practice


Basic Unix commands were practiced to understand file system navigation and file handling.


Commands practiced include:


- `pwd`, `ls` – check current directory and list files
- `mkdir`, `cd` – create and move between directories
- `echo`, `cat` – create and view text files
- `wc` – count lines, words, and characters
- `grep` – search for patterns in files
- `cp`, `mv`, `rm` – copy, move, and delete files


A simple text file was created and modified to practice searching and counting text using Unix utilities.


---


## FASTA File Practice


FASTA is a standard file format in bioinformatics used to store nucleotide or protein sequences.


### Sample FASTA File


A small FASTA file (`sample.fasta`) was manually created to understand FASTA structure.


FASTA format basics:
- Each sequence starts with a header line beginning with `>`
- Sequence data follows the header


Commands used:
```bash
grep ">" sample.fasta
grep ">" sample.fasta | wc -l
grep -v ">" sample.fasta | wc -c
Real Biological FASTA Data

Real biological FASTA files were analyzed:

tb1.fasta (DNA)

tb1-protein.fasta (Protein)

tga1-protein.fasta (Protein)

Analyses performed:

Viewing FASTA headers using head

Counting number of sequences using grep and wc

Estimating total nucleotide or amino acid count

Comparing file sizes using ls -lh

These checks are commonly performed before downstream bioinformatics analyses.

FASTA Analysis Results

The results of FASTA file analysis are documented in:

results/fasta_analysis_results.txt

This file records:

Number of sequences per FASTA file

Total nucleotide or amino acid counts

File sizes and basic observations

Conclusion

This mini project strengthened practical Unix skills essential for bioinformatics.
It demonstrates how simple Unix commands can efficiently analyze biological sequence data and form the foundation of larger bioinformatics workflows.
