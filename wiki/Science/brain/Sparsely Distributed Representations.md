---
aliases:
  - SDR
  - SDRs
tags:
  - brain
  - sci
  - bio
  - theory
web-links: https://discourse.numenta.org/t/sparse-distributed-representations/2150
category:
  - Science
---
- beautiful idea. 
	- **Distributed Semantics:** Meaning is not stored in a single specific bit, but is spread across the entire active population. Each active bit represents a specific semantic attribute or feature of the data. 
	- **Robustness to Noise and Damage:** Because information is distributed, losing or altering a few bits (subsampling or noise) does not destroy the overall meaning, allowing the system to recognize patterns despite errors
	- **Overlap and Similarity:** Comparing two SDRs via a bitwise overlap (intersection) instantly reveals how much semantic meaning they share; a high number of overlapping active bits indicates high similarity
	- **Union Operations:** Combining multiple SDRs using a bitwise OR operation creates a composite representation that preserves group semantic properties, making it useful for simultaneous predictions or overlapping memories.
- see [HTM](wiki/Science/brain/Hierarchical%20Temporal%20Memory.md)
- an idea of representation in the [Neocortex](wiki/Science/brain/Neocortex.md)

---
## what?
**Sparse Distributed Representations (SDRs)** are high-dimensional binary vectors where only a very small fraction of the bits are active (set to 1) at any given time, and the semantic meaning of the data is distributed across these active bits. [[1](https://www.youtube.com/watch?v=8GqVvDR6IzA&t=425), [2](https://www.emergentmind.com/topics/sparse-distributed-representation), [3](https://www.youtube.com/watch?v=iNMbsvK8Q8Y&t=287)]

Inspired by how the mammalian brain and neocortex encode information via populations of neurons, SDRs serve as a foundational data structure in frameworks like Hierarchical Temporal Memory ([HTM](Hierarchical%20Temporal%20Memory.md))

## Core Properties of SDRs

- **Semantic Meaning:** Unlike traditional computer codes (like ASCII) where bit positions are arbitrary, each bit in an SDR represents a specific elemental feature or attribute of the data. [](https://www.youtube.com/watch?v=iNMbsvK8Q8Y&t=287)
    
    ![](https://www.youtube.com/watch?v=iNMbsvK8Q8Y&t=287)

- **Built-in Similarity (Overlap):** Comparing two SDRs via bitwise overlap (counting shared active bits) instantly reveals how semantically similar two concepts are. [https://discourse.numenta.org/t/sparse-distributed-representations/2150](https://discourse.numenta.org/t/sparse-distributed-representations/2150)

- **High Capacity:** Despite low activity levels (e.g., 40 active bits out of 2,048), the combinatorial math yields an astronomically massive number of unique representable patterns. ![](https://www.youtube.com/watch?v=LbZtc_zWBS4&t=835)

- **Robustness & Noise Tolerance:** If an SDR is partially corrupted, missing bits, or superimposed with noise, the system can still accurately recognize the underlying pattern. [see the Wikipedia article on SDRs](https://en.wikipedia.org/wiki/Sparse_distributed_memory)

- **Union Operations:** Combining multiple SDRs using a bitwise OR operation allows a system to represent multiple simultaneous predictions or composite concepts efficiently. ![](https://www.youtube.com/watch?v=iNMbsvK8Q8Y&t=287)

## Benefits Over Dense Embeddings

- **Enhanced Interpretability:** The sparse, structured nature of active bits makes it easier to inspect and understand what features trigger a representation. [https://seanpedersen.github.io/posts/sparse-distributed-representations/](https://seanpedersen.github.io/posts/sparse-distributed-representations/)

- **Energy and Storage Efficiency:** Storing only the indices of active nonzero components significantly reduces memory footprints and processing overhead during associative retrieval. [www.sciencedirect.com/science/article/pii/S0925231226005655](https://www.sciencedirect.com/science/article/pii/S0925231226005655)
