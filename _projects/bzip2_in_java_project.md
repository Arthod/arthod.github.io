---
layout: page
title: Bachelor Thesis on bzip2 Compression Software
description: Implementation and analysis of the bzip2 compression pipeline in Java.
importance: 1
category: former
related_publications: false
---

[bzip2](https://sourceware.org/bzip2/) is a widely used lossless compression program that achieves high compression ratios through a pipeline of transformations, most notably the Burrows–Wheeler Transform (BWT) [[1]](#1), followed by Move-To-Front (MTF) encoding, Run-Length Encoding (RLE), and Huffman coding [[2]](#2). In particular, the compression process can be described as:

**RLE -> BWT → MTF → RLE → Huffman coding**

This pipeline improves compressibility by first rearranging input data into runs of similar symbols (BWT), then exploiting locality (MTF), compressing repeated patterns (RLE), and finally applying entropy coding (Huffman).

My bachelor thesis focused on implementing the bzip2 compression and decompression pipeline in Java, and analyzing the performance and contribution of the individual components to the overall compression process. We further experiment with different configurations to the standard pipeline and suggest improvements to the algorithm while retaining backwards compatibility.

The thesis was supervised by Prof. [Rolf Fagerberg](https://imada.sdu.dk/u/rolf/).

## Thesis and Source Code

- Thesis available [here](/assets/pdf/ahmadothman-bachelorproject.pdf) in pdf.
- Implementation can be found in the GitHub repository [Bzip2-in-Java](https://github.com/Arthod/Bzip2-in-Java).

## References

<a id="1">[1]</a> 
Michael Burrows and David Wheeler. *A block-sorting lossless data compression algorithm*. SRS Research Report 124 (1994).

<a id="2">[2]</a> 
David A. Huffman. *A method for the construction of minimum-redundancy codes*. Proceedings of the IRE, 40(9):1098–1101, 1952.