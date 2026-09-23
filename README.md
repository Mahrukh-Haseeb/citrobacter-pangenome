# Pangenome and Phylogenomic Analysis of *Citrobacter freundii*

Independent analysis of 188 *Citrobacter freundii* genomes from NCBI, characterizing pangenome structure, core genome phylogeny, and antimicrobial resistance (AMR) gene distribution.

## Key Findings
- **Open pangenome:** Heaps' law α = 0.714 (R² = 0.9999)
- **Pangenome composition:** 26,080 total genes; 3,397 core (13.0%), 20,053 cloud (76.9%)
- **Phylogeny:** 188-genome core tree (3,492 genes, 3.66M sites), GTR+F+I+G4, 1,000 UFBoot replicates
- **AMR:** 2,272 resistance gene hits; **blaKPC-2 in 22% of genomes** with a non-clonal distribution

## Data
188 *C. freundii* genomes from NCBI RefSeq/GenBank. After collapsing RefSeq/GenBank duplicates (408 → 220) and removing one misidentified *C. portucalensis*, 188 genomes were retained.

## Methods
| Step | Tool |
|------|------|
| Annotation | Prokka v1.14.6 |
| Pangenome | Panaroo v1.3 (strict clean mode) |
| Openness | Heaps' law (custom Python) |
| Phylogeny | IQ-TREE v3.1.3 (GTR+F+I+G4, 1,000 UFBoot) |
| AMR screening | AMRFinderPlus v4.2.7 |
| Visualization | iTOL v6 |

## Files
| File | Description |
|------|-------------|
| `combined_amr_final.tsv` | All AMR gene hits per genome |
| `summary_statistics.txt` | Pangenome core/cloud statistics |
| `itol_amr_annotation.txt` | iTOL binary dataset |
| `consensus_tree.nhx` | Final phylogenetic tree |
| `genome_list.txt` | 188 genome accessions |
| `Figure_2_AMR_tree.pdf` | Core genome tree with AMR overlay |

## Status
Manuscript in preparation.
