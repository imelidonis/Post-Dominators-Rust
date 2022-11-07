# Implementation of Post-Dominators Analysis for the Rust Compiler

BSc. Thesis, Computer Science Department, University of Crete

## Abstract

Increased demand for reliable, safe and efficient software has led to modern programming languages aiming to incorporate these principles as part of their core, using Static Code Analysis. One of these languages is Rust. Static Code Analysis is the analysis of source code during compilation instead of a run-time environment. This study shows the process of integrating Post-Dominators Analysis into the Rust Compiler and provides a better understanding of the compiler and how it handles static analysis. Post-Dominators Analysis is a Backward Control-Flow Static Analysis providing information to other analyzers and optimizers. It finds for each point of execution of a function, which other parts is certain that they will run in the future.

For the evaluation, the Rust Compiler source code is used as the code base for the measurements, because it is one of the largest software written in Rust and thus it is a representative sample. The source code was compiled by the rustc version that includes the Post-Dominators Analysis. All metrics were extracted by using a function inside the compiler that took the role of the consumer for the analysis. The evaluation is focused on what types of graphs the compiler is processing in general and how the structure of analyzed graphs affects the result of Post-Dominators Analysis.

## Implementation

- [post-dominators-analysis](https://github.com/imelidonis/rust/tree/post_dominators_analysis)
