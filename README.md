# Binary Search Trees and Red-Black Trees

An educational comparison of an ordinary binary search tree and a red-black
tree, implemented in Python. The experiments investigate how random and ordered
input affect insertion and search timings.

## What is included

| File | Purpose |
| --- | --- |
| [Tree.py](Tree.py) | Nodes, the `ABR` binary search tree, and the `RB` red-black tree |
| [Test.py](Test.py) | Repeated timing experiments and comparison plots |

The `ABR` class includes insertion, lookup, traversal, extrema, and deletion
methods. The red-black implementation adds color-aware balancing logic. The
experiment driver compares insertion and search in both structures and also
measures deletion of ordered input in the ordinary BST.

## Getting started

Use an isolated **Python 2.7** environment with compatible Matplotlib.
The source uses Python 2 `print` statements and mutable `range` results, so it
does not run unchanged under Python 3. Python 2 is end-of-life.

From the repository root:

```sh
python2 Test.py
```

The script runs the experiments, writes timing data to `m1.p` through `m9.p`,
and displays several plots. Close plot windows to continue through the results.

## Reading the experiments

The benchmarks use generated integer arrays and repeat each measurement before
averaging. Ordered input is particularly useful for studying the difference
between an unbalanced tree and a balancing strategy.

`ABR` is the original Italian abbreviation for a binary search tree.
The scripts and diagnostic output retain their original names and language.
These are historical learning implementations, not a validated production
container library. Only load trusted pickle files.

## Project provenance

This repository is a fork of
[edoardore/Red-Black-Tree](https://github.com/edoardore/Red-Black-Tree).
The original source and history are preserved.
