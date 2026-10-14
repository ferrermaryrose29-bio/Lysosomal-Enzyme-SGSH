# Lysosomal Enzyme Analysis: SGSH

**Enzyme:** N-sulfoglucosamine sulfohydrolase (sulfamidase)
**Gene symbol:** SGSH
**NCBI protein record:** [NP_000190.1](https://www.ncbi.nlm.nih.gov/protein/NP_000190.1)

## Brief function description

SGSH is a lysosomal sulfatase that helps break down heparan sulfate, a long sugar chain found on cell surfaces and in the extracellular matrix. It removes the sulfate group from the glucosamine sugar at the non-reducing end of the chain, which lets other lysosomal enzymes continue degrading the rest of it. The protein record I used is the full-length human RefSeq isoform 1 precursor, which is 502 amino acids long.

## Figures

**Figure 1.** Amino acid composition of SGSH.

![Figure 1: amino acid composition of SGSH](figures/SGSH_amino_acid_composition.png)

**Figure 2.** Positions of the potential N-glycosylation motifs (N-X-S/T, where X is not P) along the SGSH protein.

![Figure 2: potential N-glycosylation motifs in SGSH](figures/SGSH_potential_N_glycosylation.png)

## Answers to the five questions

**1. What does your enzyme normally break down inside lysosomes?**

SGSH normally breaks down heparan sulfate inside lysosomes. It removes the sulfate group from the glucosamine sugar at the non-reducing end of the heparan sulfate chain, so the other lysosomal enzymes can keep breaking the chain down into smaller pieces.

**2. What is the total length of your protein, and which amino acids are most common?**

The SGSH protein is 502 amino acids long. The most common amino acid is leucine (L) with 61 residues, which is 12.15% of the protein. Next is proline (P) with 40 residues (7.97%), then alanine (A) with 34 residues (6.77%). Glycine (G) and serine (S) are tied after that with 33 residues each (6.57%).

**3. How many potential N-glycosylation motifs did you find? Where are they located?**

I found 5 potential N-glycosylation motifs (N-X-S/T, where X is not proline) in SGSH. They start at positions 41 (NNS), 142 (NGS), 151 (NIT), 264 (NDT), and 413 (NRT). They are spread along the protein, with one near the N-terminal end, two close together around positions 142 and 151, one near the middle at 264, and one near the C-terminal end at 413.

**4. Why can glycosylation matter for lysosomal proteins? Does finding a motif prove the protein is glycosylated?**

Glycosylation matters for lysosomal proteins because it can help them fold correctly and stay stable, and some N-linked glycans can be modified with a mannose-6-phosphate tag that helps send the enzyme to the lysosome instead of out of the cell. Finding an N-X-S/T motif does not prove the protein is glycosylated. It only shows that the sequence has the right pattern, and the site could still be unused, buried inside the protein, or not modified in the cell. Showing real glycosylation would need experimental evidence.

**5. What could happen in the cell if your enzyme did not work properly?**

If SGSH did not work properly, heparan sulfate would not be fully broken down and would build up inside the lysosomes. In humans this causes mucopolysaccharidosis type IIIA (Sanfilippo syndrome A), a lysosomal storage disease that mostly affects the brain and nervous system.

## Note

N-X-S/T is only a potential N-glycosylation motif. It does not confirm that a glycan or a mannose-6-phosphate tag is present, and protein sequence analysis does not directly measure enzyme activity.

## Files in this repository

The R script `lysosomal_enzyme_analysis.R` downloads the sequence from NCBI and creates the output files. The `data/` folder has the FASTA sequence, the `results/` folder has the summary, amino acid counts, and motif positions as CSV files, and the `figures/` folder has the two figures shown above.

