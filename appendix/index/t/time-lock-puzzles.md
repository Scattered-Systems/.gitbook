# Time-lock Puzzles

## Overview

> Time-lock puzzles are elegant protocols that enable a party to lock a message such that no one else can unlock it until a certain time elapses.

### A Multi-Instance Publicly Verifiable Time-Lock Puzzle

{% embed url="https://iohk.io/en/research/library/papers/multi-instance-publicly-verifiable-time-lock-puzzle-and-its-applications/" %}

Time-lock puzzles have led to the advent of several useful technologies, enabling a party to freeze or lock a message such that no one else can unlock it until the specified time has elapsed. That being said, current systems are ill suited for practical use, being limited in their ability to process multiple instances of the puzzle that are given to the respective server all at once and expected to unlock across different points in time. In this case, existing solutions attempt to solve each puzzle at once, imposing a significant amount of overhead given the high degree of parallelization thus exponentiating the computational cost. Researchers at IOHK managed to formally define a multi-instance time-lock puzzle which general allows for the composition of a puzzle's instances. The proposed construction, _chained time-lock puzzle (C-TLP),_ allows servers, given the composition, to solve puzzles sequentially without requiring parallel computations to be invoked. Additionally, the formalized protocol makes black-box use of a standard time-lock puzzle scheme and is accompanied by a lightweight publicly verifiable algorithm. C-TLP is then leveraged to develop so-called outsourced proofs of retrievability. These proof of retrievability can support the real-time detections and fair payment while further reducing the overhead required for the execution of any given puzzle.

