---
title: "Clock2Q+: Correlation-Aware Metadata Caching Replacement Algorithm for Enterprise Storage Systems"
excerpt: "Production-oriented cache replacement algorithm for VMware vSAN.<br/><img src='/images/clock2qplus.png' width='500'>"
collection: portfolio
permalink: /portfolio/clock2qplus
---

Metadata caches show correlated references that trick LRU/2Q/CLOCK/S3-FIFO into marking blocks “hot.” Clock2Q+ uses three queues + a correlation window so near-duplicate hits don’t set the reference bit.

* Characterized metadata correlation across block-cache datasets (e.g., B-tree leaves).
* Designed/implemented Clock2Q+ for high-locality requests.
* Observed up to 28.5% miss-ratio reduction on metadata traces; wins carry to data traces.

<figure>
    <img src="/images/clock2qplus.png" alt="Clock2Q+ Illustration" width="400" />
        <figcaption>Clock2Q+ maintains three queues to separate correlated and uncorrelated accesses.</figcaption>
</figure>

<figure>
    <img src="/images/clock2qplus_res.png" alt="Clock2Q+ Results" />
    <figcaption>Clock2Q+ outperforms LRU, 2Q, CLOCK, and S3-FIFO on both data and metadata traces.</figcaption>
</figure>