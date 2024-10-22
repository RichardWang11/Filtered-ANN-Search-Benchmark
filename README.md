# Vector-Search-Benchmark&Datasets
   a benchmark contains all vecor searchs (include dense vector, sparse vector, filter vector search...)
# Benchmarks
## Billion-scale BigANN benchmarks
### Results of the Big ANN: NeurIPS’23 competition(https://arxiv.org/pdf/2409.17424)
*Track 1: *Filtered Search Track*
*Track 2: *Out-Of-Distribution(OOD) Track*
       The query vectors and vectors in database have different distributions in the share vector space.
   ![image](https://github.com/RichardWang11/Vector-Search-Benchmark/blob/main/OODtrack.png)
*Track 3: *Sparse Track*
      Given a sparse query vector, the index should return the top-k results according to the maximal inner product between the vectors.
*Track 4: *Streaming Track*
      While in practice such indices must support concurrent operations, we allow the index to batch process one class of operations at a time for simplicity. The index startswith zero points and must implement a “runbook” – a sequence of batches of insertion operations, deletion operations, and search commands in a ratio of roughly 4:4:1.

### CANDY (https://arxiv.org/pdf/2406.19651)
   A Benchmark for Continuous Approximate Nearest Neighbor Search with Dynamic Data Ingestion
   Evaluating vector search performance to adapt to changing data pattern, integrating new optimizations (e.g. ML-driven inference) to replace traditional heuristic scans, and improved distance computation methods.
### Datasets
Reference this paper, we category the datasets into 5 types (https://ieeexplore.ieee.org/abstract/document/8681160):

| Name   | n (×10^3) | d    | RC   | LID  | Type       |
|--------|-----------|------|------|------|------------|
| Nus*   | 269       | 500  | 1.67 | 24.5 | Image      |
| Gist*  | 983       | 960  | 1.94 | 18.9 | Image      |
| Rand*  | 1,000     | 100  | 3.05 | 58.7 | Synthetic  |
| Glove* | 1,192     | 100  | 1.82 | 20.0 | Text       |
| Cifa   | 50        | 512  | 1.97 | 9.0  | Image      |
| Audio  | 50        | 192  | 2.97 | 5.6  | Audio      |
| Mnist  | 69        | 784  | 2.38 | 6.5  | Image      |
| Sun    | 79        | 512  | 1.94 | 9.9  | Image      |
| Enron  | 95        | 1,369| 6.39 | 11.7 | Text       |
| Trevi  | 100       | 4,096| 2.95 | 9.2  | Image      |
| Notre  | 333       | 128  | 3.22 | 9.0  | Image      |
| Yout   | 346       | 1,770| 2.29 | 12.6 | Video      |
| Msong  | 922       | 420  | 3.81 | 9.5  | Audio      |
| Sift   | 994       | 128  | 3.50 | 9.3  | Image      |
| Deep   | 1,000     | 128  | 1.96 | 12.1 | Image      |
| Ben    | 1,098     | 128  | 1.96 | 8.3  | Image      |
| Gauss  | 2,000     | 512  | 3.36 | 19.6 | Synthetic  |
| Imag   | 2,340     | 150  | 2.54 | 11.6 | Image      |
| UQ-V   | 3,038     | 256  | 8.39 | 7.2  | Video      |
| BANN   | 10,000    | 128  | 2.60 | 10.3 | Image      |




SIFT1M,SIFT100M; Deep1M; GIST1M;Msong;Audio;UQ-V;Crawl;GloVe;Enron
    
