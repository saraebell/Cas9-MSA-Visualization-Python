# Cas9-in-Two-Taxonomic-Orders-of-Bacteria-Python
# Methods

Heatmap and plots will be generated to better help visual the sequence data:


1. A multiple sequence alignment (MSA) was created using the complete Cas9 protein sequence from 50 species. The MSA was used to select a conserved region for experimental purposes.

2. Two datasets used to build HMMs were downloaded using blastp from NCBI. The accession number WP_032462936 for S. pyogenes was used in this report as the query sequence to obtain complete Cas9 sequences.All sequences collected fall within the taxonomic class ‘Bacilli’.

3. The two dataset were separated by taxonomic order: Lactobacillales (taxid:186826) and Bacillales (taxid:1385). The first dataset collected consisted of 25 sequences from species in the order Lactobacillales. The second dataset collected consisted of 25 sequences from species in the order Bacillales.  

4. Settings for collecting both datasets were identical except for the ‘Organism’ setting under ‘Choose Search Set’. The algorithm used was ‘blastp’. To find non-redundant, well-annotated, and curated sequences, the database ‘RefSeq Select proteins (refseq_select)’ was 
used. To obtain more hits, the ‘Max target sequences’ was selected as 500. The ‘Expect threshold’ was set at .05. When considering the alignment, ‘Word size’ was set to 6. The default ‘Matrix’ setting of ‘BLOSUM62’ was used. All other parameters were left at their default setting. 

5. The online platform Phylogeny.fr was used to generate all phylogenetics trees with bootstrap values. For phylogeny analysis, the ‘One Click’ mode with default settings was used. Clustal Omega, a public and online available program, was use to generate multiple sequence alignments in this report. Additionally, Clustal Omega was used to align the training sequences of each dataset used to build the HMMs. The output format for the alignments was “Pearson/FASTA. The java application ‘hmm2021.jar’ created by Dr. Philip Heller was used to build the Lactobacillales HMM and the Bacillales HMM. 


6. All programming to create visual graphics and plots was done on Google Collaboratory using the programming language Python. All lines of code can be found in the file ‘Bell-Sara_Cas9_Project.ipynb’. The library ‘pandas’ was imported to create Pandas DataFrames for organizing data before plotting. The library ‘Seaborn’ and ‘Matplotlib’ were imported for  data visualization. Biopython was installed in order to import ‘Seq’ and ‘SeqIO’, both of which were used to open and work with fasta files. 



 
