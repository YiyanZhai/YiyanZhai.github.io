---
title: "Clock2Q+: A Simple and Efficient Replacement Algorithm for Metadata Cache in VMware vSAN"
collection: publications
permalink: /publication/2025-11-clock2q-plus
# excerpt: ''
date: 2026-8-15
venue: 'VLDB 2026 (Industrial Track)'
# slidesurl: ''
paperurl: 'https://arxiv.org/abs/2511.21958'
# citation: ''
---

Cache replacement algorithms are vital for storage systems. We observe that metadata caches have a distinctive characteristic: correlated references, even when the corresponding data accesses do not contain correlated references. This correlation issue causes references to often be mistakenly categorized as hot blocks. To address this, Clock2Q+ introduces a three-queue design similar to S3-FIFO but adds a correlation window in the Small FIFO queue, where blocks in this window do not set the reference bit.

Clock2Q+ achieves up to a 28.5% lower miss ratio on metadata traces compared to S3-FIFO. The algorithm is designed for production use, offering low CPU overhead, minimal memory requirements, efficient multi-CPU scaling, and ease of implementation. It outperforms existing algorithms on both metadata and data traces, and has been deployed in VMware's vSAN and VDFS storage products.
