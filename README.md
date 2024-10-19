# Different repos

## Layout
- Make a folder containing the name
- Provide a github submodule referencing a specific commit (if there is a github link to repo), otherwise, just copy pasta entire repo or place http link in README
- Provide README.md containing
  - Why the repo is interesting to look into, one sentence
  - If you have impressions about the repo before looking at it, list them
    - Ex, I've heard that vLLM is good at throughput and can scale on multiple GPUs
    - Ex, Oh, rocksdb runs really well. It basically beats btree systems
  - Background
    - Ex, vLLM, probably need to know these terms: prefill, kv cache, expected latency/latency given naive kv cache, why is throughput important and in which scenarios
  - Summary of repo
  - Why did they design the repo the way it is? Is there a better way to organize? Explain
  - For certain functions/modules, do they list what they tried and didn't do? If not, think of alternatives and why you shouldn't use your idea and used their algorithm
    - For example, vLLM is adds speculative decoding in a certain way. Should they have done it this way? Why didn't they add like what is described in the original paper?
  - Does the repo match your impressions?
    - Oh, vLLM doesn't scale to multiple GPUs, it's only targetted for single GPU
    - Wait, reads on rocksdb sucks under X conditions
  - Running it
    - Throughput/Latency
      - End-to-end system
      - resource breakdown (memory/storage/compute)
        - is bandwidth saturated for each resource?
        - where is the bottleneck?
  - Strengths
    - Ex, running it is very easy!
    - Ex, the code base is simple to follow
  - Weaknesses
    - Dude, I can't run this code
    - Benchmarking code is wrong/unrealistic
  - Comparison to other related repos
    - Is this one faster?
    - Is this one easier to follow and why?
    - Can add another repo to list 

### Looked into

### To look into

* Pytorch
* Trition
* vLLM
* LevelDB
* RocksDB
* Postgres
* Milvus
* Linux kernel
* NVIDIA kernel


