# Filtered-Vector-Search-Benchmarks & Datasets
Including recently high-dim filtered vector search methods and datasets.

# Filter ANNS Papers & Methods
## Methods
- ACORN
- CAPS
- FilteredVamana
- StitchedVamana
- 2D-Segment Graph: it introduces a segment graph that compresses multiple graph-based indexes into a single structure, reducing memory consumption while maintaining high query performance for range filtered ANNS.
- SuperPostFilter: it proposes a tree-based framework to efficiently solve the c-approximate window search problem.
- NHQ:
- [HSIG](https://arxiv.org/abs/2412.02448):
- NGT:is an ANNS library developed by Yahoo Japan that processes hybrid queries using the post-filtering strategy.
- Vearch: is a high-dimensional vector retrieval system developed by Jingdong that supports hybrid queries through the post-filtering strategy.
- ADBV:is a hybrid analytic engine developed by Alibaba. It enhances PQ for hybrid ANNS and proposes the accuracy-aware, cost-based optimization to generate optimal execution plans.
- Milvus: partitions datasets based on commonly utilized attributes and implements ADBV within each subset.
# Datasets
Referring to this [paper](https://ieeexplore.ieee.org/abstract/document/8681160), we categorize the datasets into eight types, which *RC (Relative Contrast)* is mean average distance / nearest neighbor distance, the smaller RC means the dataset is harder; *LID (Local Intrinsic Dimensionality)* the high LID means the dataset is hard to process:
## Dense Vector Datasets
| Name   | n (×10^3) | d    | RC   | LID  | Category  |Distance|
|--------|-----------|------|------|------|------------|------------|
| Nus   | 269       | 500  | 1.67 | 24.5 | Image      |L2|
| Gist  | 983       | 960  | 1.94 | 18.9 | Image      ||
| Rand  | 1,000     | 100  | 3.05 | 58.7 | Synthetic  ||
| [Glove](https://github.com/stanfordnlp/GloVe) | 1,192     | 100  | 1.82 | 20.0 | Text       ||
| Cifa   | 50        | 512  | 1.97 | 9.0  | Image      ||
| Mnist  | 69        | 784  | 2.38 | 6.5  | Image      |L2|
| Sun    | 79        | 512  | 1.94 | 9.9  | Image      ||
| Enron  | 95        | 1,369| 6.39 | 11.7 | Text       |L2|
| Trevi  | 100       | 4,096| 2.95 | 9.2  | Image      ||
| Notre  | 333       | 128  | 3.22 | 9.0  | Image      ||
| [SIFT](http://corpus-texmex.irisa.fr/)| 994       | 128  | 3.50 | 9.3  | Image      |L2|
| Deep1M   | 1,000     | 128  | 1.96 | 12.1 | Image      |L2|
| Ben    | 1,098     | 128  | 1.96 | 8.3  | Image      ||
| Gauss  | 2,000     | 512  | 3.36 | 19.6 | Synthetic  ||
| Imag   | 2,340     | 150  | 2.54 | 11.6 | Image      ||
| BANN   | 10,000    | 128  | 2.60 | 10.3 | Image      |L2|
| Audio  | 50        | 192  | 2.97 | 5.6  | Audio      ||
| Msong  | 922       | 420  | 3.81 | 9.5  | Audio      ||
| Yout   | 346       | 1,770| 2.29 | 12.6 | Video      ||
| UQ-V   | 3,038     | 256  | 8.39 | 7.2  | Video      ||
| [Kosarak](http://fimi.uantwerpen.be/data/)| 75 | 27983 | - | -  | -     |Jaccard|
|[NYTimes](https://archive.ics.uci.edu/dataset/164/bag+of+words)|256| 290 | - | -  | Text|Angular|
|[Fashion-MNIST](https://github.com/zalandoresearch/fashion-mnist)|60|784| - | -  | Image|L2|


## Filtered Dataset
| Name   | Dim | Data-Type  |Category|Distance|
|--------|-----------|------|------|------|
| YFCC-10M + CLIP| 192| uint8|Image|L2|
| [Words](https://huggingface.co/datasets/efarrall/word_embeddings/tree/main)| 3072| float|Text||
| [MTG](https://huggingface.co/datasets/TrevorJS/mtg-scryfall-cropped-art-embeddings-open-clip-ViT-SO400M-14-SigLIP-384)| 1152| float| Image||
| [WIT-Image](https://www.kaggle.com/c/wikipedia-image-caption/data)| 1024| float| Image||
| [Youtube-Audio](https://research.google.com/youtube8m/download.html) | 128| float| Audio||
| [YouTube-RGB](https://research.google.com/youtube8m/download.html) | 1024| float| Video||
| [TripClick](https://tripdatabase.github.io/tripclick/) ||| Text||
| [Redcaps](https://github.com/JoshEngels/RangeFilteredANN) | 512|| Multi-modality||
| [ArXiv](https://huggingface.co/datasets/malteos/aspect-paper-embeddings) | 768| float| Text||

## Deep Learning Datasets
| Name   | n (×10^3) | d    |Category|Distance|
|--------|-----------|------|------|------|
|[DRP10M](https://github.com/IntelLabs/VectorSearchDatasets/tree/main/dpr)|10,000|768| Text|IP|
|[Open-images13M](https://github.com/IntelLabs/VectorSearchDatasets/tree/main/dpr)|13,000|512| Image|IP|
|[RQA10M](https://github.com/IntelLabs/VectorSearchDatasets/tree/main/dpr)|10,000|768| Text|IP|
|[WIT1M](https://github.com/IntelLabs/VectorSearchDatasets/tree/main/dpr)|1,000|512| Cross-Model|IP|
    
# Other useful links
## [PQ-based variants](https://raw.githubusercontent.com/wiki/facebookresearch/faiss/PQ_variants_Faiss_annotated.png)
## [Speach of NeurIPS'21 competition](https://neurips.cc/virtual/2023/competition/66587)
## Additional Benchmarks
- [Vector Filtering Benchmarks](https://github.com/qdrant/ann-filtering-benchmark-datasets)
- [DBWangGroupUNSW_NNS_Benchmark](https://github.com/DBAIWangGroup/nns_benchmark)
- Xinjing Hu, Xuanhua Shi, Shixuan Sun, et al. CANDY: A Benchmark for Continuous Approximate Nearest Neighbor Search with Dynamic Data Ingestion. arXiv preprint arXiv:2406.19651 (2024)[[github](https://github.com/intellistream/CANDY-Benchmark)][[paper](https://arxiv.org/pdf/2406.19651)]
