 Oil Palm Stress Response Transcriptomic Analysis
 Project Overview
RNA-seq analysis of oil palm (Elaeis guineensis) under stress conditions compared to control samples. This study identifies differentially expressed genes and provides insights into the molecular mechanisms of stress response.

 Analysis Summary

 Key Findings
- Total significant DEGs: 2,253 genes (FDR < 0.05 & |log2FC| > 1)
- Up-regulated in stress: 1,090 genes
- Down-regulated in stress: 1,163 genes
- Total genes analyzed: 23,531 genes

 Top Significant Genes
| Gene ID | Log2FC | Direction | P-value |
|---------|--------|-----------|---------|
| LOC109505290 | -7.72 | Down | 2.15e-85 |
| LOC105051082 | -4.10 | Down | 6.30e-75 |
| LOC105036436 | +6.87 | Up | 8.67e-74 |
| LOC109504909 | -4.92 | Down | 2.51e-68 |

 Methods
 Experimental Design
- Control samples: OPS_CONTROL_R2, OPS_CONTROL_R3
- Stressed samples: OPS_STRESSED12D_R2, OPS_STRESSED12D_R3
- Replicates: 2 biological replicates per condition

 Bioinformatics Pipeline
1. Quality Control: FastQC & MultiQC
2. Trimming: fastp
3. Alignment: STAR
4. Quantification: featureCounts
5. Differential Expression: DESeq2 (R package)
6. Visualization: ggplot2, pheatmap, ComplexHeatmap

 Statistical Analysis
- Differential expression: DESeq2 (negative binomial model)
- Multiple testing correction: Benjamini-Hochberg (FDR)
- Significance threshold: padj < 0.05 & |log2FC| > 1
- Normalization: Variance Stabilizing Transformation (VST)

