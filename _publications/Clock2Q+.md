---
title: "Clock2Q+: A Simple and Efficient Replacement Algorithm for Metadata Cache in VMware vSAN"
collection: publications
permalink: /publication/2025-11-clock2q-plus
excerpt: "Production-oriented cache replacement algorithm for VMware vSAN.<br/><img src='/images/clock2qplus.png' width='500'>"
date: 2026-8-15
venue: 'VLDB 2026 (Industrial Track)'
paperurl: 'https://arxiv.org/abs/2511.21958'
# citation: ''
---

Metadata caches show correlated references that trick LRU/2Q/CLOCK/S3-FIFO into marking blocks "hot." Clock2Q+ uses three queues + a correlation window so near-duplicate hits don't set the reference bit.

* Characterized metadata correlation across block-cache datasets (e.g., B-tree leaves).
* Designed/implemented Clock2Q+ for high-locality requests.
* Observed up to 28.5% miss-ratio reduction on metadata traces; wins carry to data traces.

Clock2Q+ is designed for production use, offering low CPU overhead, minimal memory requirements, efficient multi-CPU scaling, and ease of implementation. It outperforms existing algorithms on both metadata and data traces, and has been deployed in VMware's vSAN and VDFS storage products.

<figure>
    <img src="/images/clock2qplus.png" alt="Clock2Q+ Illustration" width="400" />
    <figcaption>Clock2Q+ maintains three queues to separate correlated and uncorrelated accesses.</figcaption>
</figure>

<figure>
    <img src="/images/clock2qplus_res.png" alt="Clock2Q+ Results" />
    <figcaption>Clock2Q+ outperforms LRU, 2Q, CLOCK, and S3-FIFO on both data and metadata traces.</figcaption>
</figure>
