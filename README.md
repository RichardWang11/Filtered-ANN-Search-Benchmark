# Advanced-Vector-Search-Benchmarks & Datasets
   Containing almost high dimentional vector search approaches include dense vector search, sparse vector search, and filter vector search...
# Benchmarks
## [FAISS](https://github.com/facebookresearch/faiss)
## Billion-scale BigANN benchmarks
### [NeurIPS’23 competition](https://arxiv.org/pdf/2409.17424)
### Track 1: Filtered Search Track
### Track 2: Out-Of-Distribution(OOD) Track
The query vectors and vectors in database have different distributions in the share vector space. ![image](https://github.com/RichardWang11/Vector-Search-Benchmark/blob/main/OODtrack.png) 
### Track 3: Sparse Track
Given a sparse query vector, the index should return the top-k results according to the maximal inner product between the vectors.
### Track 4: Streaming Track
while in practice such indices must support concurrent operations, we allow the index to batch process one class of operations at a time for simplicity. The index startswith zero points and must implement a “runbook” – a sequence of batches of insertion operations, deletion operations, and search commands in a ratio of roughly 4:4:1.

## [Vector Filtering benchmarks](https://github.com/qdrant/ann-filtering-benchmark-datasets)
## [CANDY](https://arxiv.org/pdf/2406.19651)
A Benchmark for *Continuous Approximate Nearest Neighbor Search with Dynamic Data Ingestion* Evaluating vector search performance to adapt to changing data pattern, integrating new optimizations (e.g. ML-driven inference) to replace traditional heuristic scans, and improved distance computation methods.
## [VectorDB Benchmark](https://zilliz.com/vector-database-benchmark-tool?database=ZillizCloud%2CMilvus%2CElasticCloud%2CPgVector%2CPinecone%2CQdrantCloud%2CWeaviateCloud&dataset=medium&filter=none%2Clow%2Chigh&tab=1)
VectorDBBench provides unbiased vector database benchmark results for mainstream vector databases and cloud services.
### Database
Zilliz Cloud;Milvus;Elastic Cloud;PgVector;Pinecone;Qdrant Cloud;Weaviate Cloud
### Dataset
-Medium(Cohere1M of 768-dim vectors; OpenAI500K of 1,536-dim vectors)
-Large(Cohere10M of 768-dim vectors; OpenAI5M of 1,536-dim vectors)
### Comparison results
*QPS* shows the throughput of mainstream vector databases, showcasing their comprehensive QPS scores and rankings based on the scores, QPS, and recall rates.

*P99 Latency* demonstrates the response speed of mainstream vector databases, showcasing their comprehensive P99 latency scores and rankings based on the scores, P99 latency, and recall rates.

The *Cost* Ranking compares the cost of mainstream vector databases, detailing their cost-performance ratios, rankings based on the ratio, and dollars per one million queries.
## [MyScales's Vector Database Benchmark](https://myscale.github.io/benchmark/#/benchmark)
Update results of Zilliz Cloud (version 2024-04-03)
## [DBWangGroupUNSW_nns_benchmark](https://github.com/DBAIWangGroup/nns_benchmark)
# Datasets
Reference this [paper](https://ieeexplore.ieee.org/abstract/document/8681160), we category the datasets into 8 types:

| Name   | n (×10^3) | d    | RC   | LID  | Type       |Distance|
|--------|-----------|------|------|------|------------|------------|
| Nus*   | 269       | 500  | 1.67 | 24.5 | Image      |L2|
| Gist*  | 983       | 960  | 1.94 | 18.9 | Image      ||
| Rand*  | 1,000     | 100  | 3.05 | 58.7 | Synthetic  ||
| Glove* | 1,192     | 100  | 1.82 | 20.0 | Text       ||
| Cifa   | 50        | 512  | 1.97 | 9.0  | Image      ||
| Mnist  | 69        | 784  | 2.38 | 6.5  | Image      |L2|
| Sun    | 79        | 512  | 1.94 | 9.9  | Image      ||
| Enron  | 95        | 1,369| 6.39 | 11.7 | Text       |L2|
| Trevi  | 100       | 4,096| 2.95 | 9.2  | Image      ||
| Notre  | 333       | 128  | 3.22 | 9.0  | Image      ||
| [SIFT](http://corpus-texmex.irisa.fr/)| 994       | 128  | 3.50 | 9.3  | Image      |L2|
| Deep   | 1,000     | 128  | 1.96 | 12.1 | Image      |L2|
| Ben    | 1,098     | 128  | 1.96 | 8.3  | Image      ||
| Gauss  | 2,000     | 512  | 3.36 | 19.6 | Synthetic  ||
| Imag   | 2,340     | 150  | 2.54 | 11.6 | Image      ||
| BANN   | 10,000    | 128  | 2.60 | 10.3 | Image      |L2|
| Audio  | 50        | 192  | 2.97 | 5.6  | Audio      ||
| Msong  | 922       | 420  | 3.81 | 9.5  | Audio      ||
| Yout   | 346       | 1,770| 2.29 | 12.6 | Video      ||
| UQ-V   | 3,038     | 256  | 8.39 | 7.2  | Video      ||
| [Kosarak](http://fimi.uantwerpen.be/data/)| 75   | 27983 | - | -  | -     |Jaccard|
| [MovieLens-10M](https://grouplens.org/datasets/movielens/10m/)| 69    | 65134 | - | -  | Online-news-portal/Click-Stream data|Jaccard|
|[NYTimes](https://archive.ics.uci.edu/dataset/164/bag+of+words)|256| 290 | - | -  | Text|Angular|
|[Fashion-MNIST](https://github.com/zalandoresearch/fashion-mnist)|60|784| - | -  | Image|L2|
|[DRP10M](https://github.com/IntelLabs/VectorSearchDatasets/tree/main/dpr)|1000|768| - | -  | Text|IP|
|[Open-images13M](https://github.com/IntelLabs/VectorSearchDatasets/tree/main/dpr)|1300|512| - | -  | Image|IP|
|[RQA10M](https://github.com/IntelLabs/VectorSearchDatasets/tree/main/dpr)|1000|768| - | -  | Text|IP|
|[WIT1M](https://github.com/IntelLabs/VectorSearchDatasets/tree/main/dpr)|100|512| - | -  | Text2Image|IP|
    
## [PQ variants](https://raw.githubusercontent.com/wiki/facebookresearch/faiss/PQ_variants_Faiss_annotated.png)
