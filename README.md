# Single-Cell-RNA-sequencing Analysis-

Goal

To demonstrate a complete scRNA-seq workflow — from preprocessing and clustering to identifying marker genes and visualizing cell-type relationships — using the PBMC3k dataset as a proxy for studying biological states such as stress or depression.

Method Overview (Top-down)

Dataset: 3,000 human Peripheral Blood Mononuclear Cells (PBMCs), a standard demo dataset in Scanpy.

Quality Control:

Filtered out cells with too few genes.

Removed cells with >5% mitochondrial content (low-quality or dying cells).

Normalization & Feature Selection:

Normalized gene counts to 10,000 per cell and log-transformed.

Selected top 2000 highly variable genes to focus on biologically informative features.

Dimensional Reduction:

Scaled data, ran PCA, computed nearest neighbors, and used UMAP for visualization.

Clustering (Leiden algorithm):

Identified communities (potential cell types) based on transcriptomic similarity.

Marker Gene Identification:

Ranked genes that best distinguish each cluster using a t-test approach.

Visualized the top 5 markers per cluster in a heatmap.

Outputs:

Cluster UMAP plot and marker gene heatmap.

CSV file with cluster assignments for downstream analyses or labeling.
