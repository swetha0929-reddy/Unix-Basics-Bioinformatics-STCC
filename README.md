# STCC – Unix Basics for Bioinformatics


## Course Documentation and Hands-on Practice  
**Student:** Thamanna Swetha Reddy  
**Institution:** Bversity School of Bioscience  


---


## Overview


Unix is an essential skill for bioinformatics and computational biology.  
This repository documents the Unix command-line concepts learned during the **Short-Term Course on Unix (STCC)** and shows how these commands are applied to **biological data analysis**, especially FASTA files.


The purpose of this repository is to clearly explain:
- What commands were used
- Why they were used
- How they are useful in bioinformatics workflows


This README is written as **learning documentation**, not just a list of commands.


---


## Learning Objectives


By completing this mini project, I demonstrate the ability to:


- Navigate the Unix/Linux file system
- Create, move, copy, and delete files and folders
- Use Unix commands to inspect biological data
- Understand and analyze FASTA sequence files
- Use Git and GitHub to manage and document work


---


## Tools and Environment


- **Operating System:** Ubuntu (WSL)
- **Shell:** Bash
- **Text Editor:** nano
- **Version Control:** Git and GitHub


---


## Unix Basics Practice


### File System Navigation


Basic Unix commands were used to move around the file system and view files.


Commands practiced:

```bash
pwd
ls
cd

Why this matters in bioinformatics:
Biological data is stored in many folders (raw data, results, scripts).
Knowing where you are and how to move between directories is essential.

Creating and Managing Files

Commands used:

mkdir
touch
cp
mv
rm

Example:

echo "Hello Unix" > example.txt
echo "Bioinformatics practice" >> example.txt
cat example.txt

Why this matters:
These commands are used to manage datasets, scripts, logs, and result files in real projects.

Searching and Counting Text

Commands practiced:

wc
grep

Examples:

wc -l file.txt
grep "gene" file.txt

Why this matters:
These commands help count sequences, genes, reads, or search for specific patterns in biological files.

FASTA File Practice

FASTA is a common file format used to store DNA and protein sequences.

Before doing any analysis, FASTA files must be checked for:

Number of sequences

Sequence length

File size

Sample FASTA File

A small FASTA file (sample.fasta) was created manually to understand the format.

FASTA structure:

Each sequence starts with >

Sequence lines follow the header

Commands used:

grep ">" sample.fasta
grep ">" sample.fasta | wc -l
grep -v ">" sample.fasta | wc -c

These commands were used to:

Count sequences

Count total nucleotides

Real Biological FASTA Files

Real biological FASTA files were analyzed:

tb1.fasta – DNA sequence

tb1-protein.fasta – Protein sequence

tga1-protein.fasta – Protein sequence

Commands used:

head tb1.fasta
grep ">" tb1.fasta | wc -l
grep -v ">" tb1.fasta | wc -c
ls -lh tb1.fasta tb1-protein.fasta tga1-protein.fasta

Purpose of these checks:

Confirm number of sequences

Estimate sequence length

Compare file sizes

Verify files before downstream analysis

These steps are standard in bioinformatics workflows.

FASTA Analysis Results

The results of FASTA analysis are saved separately in:

results/fasta_analysis_results.txt

This file contains:

Sequence counts

Nucleotide or amino acid counts

File size information

Keeping results separate from commands improves clarity and reproducibility.

Version Control with Git and GitHub

Git was used to track changes and upload the project to GitHub.

Basic workflow:

git init
git add .
git commit -m "Commit message"
git push

Why Git is important in bioinformatics:

Tracks changes

Prevents data loss

Helps collaboration

Supports reproducible research

Conclusion

This mini project helped build strong foundational skills in Unix that are essential for bioinformatics.

It demonstrates how simple Unix commands can be used to:

Navigate datasets

Inspect biological sequence files

Prepare data for larger analysis pipelines

These skills form the base for advanced work in genomics and computational biology.

Repository Information

Course: Short-Term Course on Unix (STCC)

Institution: Bversity School of Bioscience

Student: Thamanna Swetha Reddy

Purpose: Educational documentation of Unix basics for bioinformatics
