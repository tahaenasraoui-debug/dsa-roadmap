# Data Structures & Algorithms (DSA) Roadmap

![License](https://img.shields.io/badge/license-MIT-green.svg) ![language](https://img.shields.io/badge/language-python-blue.svg) ![focus](https://img.shields.io/badge/focus-interviews%20%2B%20contests-informational.svg)

A DSA-only path: fundamentals, pattern practice, proof-level rigor, contest speed, and interview execution. Volume and spaced repetition matter more than finishing any single book.

## Table of Contents

1. [Workflow Overview](#workflow-overview)
2. [Prerequisites](#prerequisites)
3. [Phase 1: Fundamentals](#phase-1-fundamentals)
4. [Phase 2: Pattern Practice](#phase-2-pattern-practice)
5. [Phase 3: Algorithmic Rigor](#phase-3-algorithmic-rigor)
6. [Phase 4: Contest Speed & Advanced Techniques](#phase-4-contest-speed--advanced-techniques)
7. [Phase 5: Interview Execution](#phase-5-interview-execution)
8. [Capstone Projects](#capstone-projects)
9. [Repository Layout](#repository-layout)
10. [Engineering Rules](#engineering-rules)
11. [Exit Criteria](#exit-criteria)

---

## Workflow Overview

```
 Complexity --> Core structures --> Pattern practice --> Rigor (proofs, DP, graphs)
                                          |                        |
                                          v                        v
                              Interview execution <-- Contest speed (Codeforces/CSES)
```

## Prerequisites

- [ ] Python basics (loops, functions, classes, built-in containers)
- [ ] High-school algebra and comfort with logs and exponents
- [ ] A LeetCode account and a Codeforces account

## Phase 1: Fundamentals

Goal: Know the cost of every operation you write and implement the core structures yourself.

| Resource | Type | Why |
|----------|------|-----|
| [Problem Solving with Algorithms and Data Structures using Python](https://runestone.academy/ns/books/published/pythonds3/index.html) | Free book | Python-first fundamentals |
| [Grokking Algorithms, 2nd Ed](https://www.manning.com/books/grokking-algorithms-second-edition) | Book | Fast visual first pass |
| [VisuAlgo](https://visualgo.net/) | Interactive | Watch structures execute step by step |
| [Python TimeComplexity wiki](https://wiki.python.org/moin/TimeComplexity) | Reference | Cost of list, dict, set, deque operations |

- [ ] Runestone: complexity, recursion, sorting, searching
- [ ] Grokking Algorithms: all chapters
- [ ] Memorize built-in container costs
- [ ] Implement dynamic array, linked list, stack, queue, hash map, binary heap

**Deliverables**
- [ ] `src/dsa/structures/` with typed implementations
- [ ] Tests for each in `tests/dsa/`
- [ ] Benchmark of your structures against the standard library in `docs/benchmarks.md`

## Phase 2: Pattern Practice

Goal: Build speed on the recurring problem patterns.

| Resource | Type | Why |
|----------|------|-----|
| [NeetCode Roadmap](https://neetcode.io/roadmap) | Curated path | Pattern ordering |
| [NeetCode 150](https://neetcode.io/practice) | Problem list | Core practice set |
| [LeetCode](https://leetcode.com/) | Platform | Volume and weekly contests |
| [Tech Interview Handbook](https://www.techinterviewhandbook.org/) | Free guide | Study plans and pattern cheat sheets |
| [TheAlgorithms/Python](https://github.com/TheAlgorithms/Python) | GitHub repo | Reference implementations to compare, not copy |

- [ ] Arrays and hashing, two pointers, sliding window, stack, binary search
- [ ] Linked lists, trees, tries, heaps, backtracking
- [ ] Graphs (BFS, DFS, topological sort, union-find)
- [ ] 1-D and 2-D DP, greedy, intervals
- [ ] Re-solve failed problems on days 3, 7, and 21

**Deliverables**
- [ ] NeetCode 150 complete
- [ ] 100 extra medium problems in `src/dsa/problems/<topic>/`
- [ ] `docs/patterns.md`: one page per pattern with the trigger signs and a template solution

## Phase 3: Algorithmic Rigor

Goal: Move from pattern matching to understanding why algorithms are correct and fast.

| Resource | Type | Why |
|----------|------|-----|
| [Algorithms (Jeff Erickson)](https://jeffe.cs.illinois.edu/teaching/algorithms/) | Free book | Recursion, DP, graphs, proofs |
| [Algorithms Illuminated (Tim Roughgarden)](https://www.algorithmsilluminated.org/) | Book series | Clear treatment of divide and conquer, graphs, greedy, DP |
| [The Algorithm Design Manual (Skiena)](https://www.algorist.com/) | Book | Catalog of problem types and which technique fits |
| [Introduction to Algorithms, CLRS](https://mitpress.mit.edu/9780262046305/introduction-to-algorithms/) | Reference textbook | Selective chapters only |

- [ ] Erickson: recursion, backtracking, DP, shortest paths, minimum spanning trees
- [ ] Algorithms Illuminated: Parts 1 to 3
- [ ] CLRS: amortized analysis, graph algorithms, NP-completeness
- [ ] Prove correctness for 5 algorithms: induction, exchange argument, loop invariant

**Deliverables**
- [ ] `docs/proofs.md` with 5 written proofs
- [ ] 20 hard problems solved with complexity analysis

## Phase 4: Contest Speed & Advanced Techniques

Goal: Learn the techniques that fall outside standard interview sets and practice under time pressure.

| Resource | Type | Why |
|----------|------|-----|
| [Competitive Programmer's Handbook](https://cses.fi/book/book.pdf) | Free PDF | Compact advanced techniques |
| [CSES Problem Set](https://cses.fi/problemset/) | Problem set | Classic problems with hidden tests |
| [cp-algorithms](https://cp-algorithms.com/) | Reference | Detailed explanations of advanced algorithms |
| [USACO Guide](https://usaco.guide/) | Free guide | Structured topic path with problems |
| [Codeforces](https://codeforces.com/) | Contest platform | Rated live contests |
| [AtCoder](https://atcoder.jp/) | Contest platform | High-quality beginner contests |

- [ ] CSES: Introductory, Sorting and Searching, Dynamic Programming, Graph, and Range Queries sections
- [ ] Learn segment trees, Fenwick trees, binary lifting, and Dijkstra with a heap
- [ ] Learn string algorithms: KMP, Z-function, rolling hash
- [ ] Compete in 10 live contests and upsolve every problem you missed

**Deliverables**
- [ ] `src/dsa/advanced/` with segment tree, Fenwick tree, and string algorithms, tested against brute force
- [ ] Contest log in `docs/contests.md` with rating and upsolve notes

## Phase 5: Interview Execution

Goal: Convert skill into a performance under observation.

| Resource | Type | Why |
|----------|------|-----|
| [Cracking the Coding Interview](https://www.crackingthecodinginterview.com/) | Book | Interview process and communication |
| [Elements of Programming Interviews in Python](https://elementsofprogramminginterviews.com/) | Book | Harder, broader problem set |
| [interviewing.io](https://interviewing.io/) | Mock interviews | Practice with engineers |
| [Pramp](https://www.pramp.com/) | Peer mock interviews | Free peer practice |

- [ ] Talk through every problem out loud: restate, examples, approach, complexity, code, test
- [ ] Do 5 timed sessions of 45 minutes with 2 problems each
- [ ] Complete 5 mock interviews and write down what went wrong

**Deliverables**
- [ ] `docs/mock_interviews.md` with feedback and fixes
- [ ] Solve a new medium in under 25 minutes without hints

## Capstone Projects

- [ ] Your own typed, tested, benchmarked data structures library, compared against the standard library
- [ ] A personal pattern handbook (`docs/patterns.md`) another learner could study from
- [ ] 300 problems solved in total, logged with complexity notes and retry dates
- [ ] Targets: a LeetCode weekly contest rating you set in advance, and a Codeforces rating you set in advance, reviewed quarterly

## Repository Layout

```
dsa/
├── README.md
├── pyproject.toml
├── src/
│   └── dsa/
│       ├── structures/       # your implementations
│       ├── advanced/         # segment tree, Fenwick, string algorithms
│       └── problems/         # one folder per topic
│           ├── arrays/
│           ├── graphs/
│           └── dp/
├── tests/                    # mirrors src/
└── docs/
    ├── dsa_log.md            # problem log: complexity, retry dates
    ├── patterns.md
    ├── proofs.md
    ├── contests.md
    ├── benchmarks.md
    └── mock_interviews.md
```

## Engineering Rules

These are strict. A phase is not complete until its deliverables follow all of them.

### 1. Daily 1:3 Theory-to-Building Ratio

- [ ] For every 1 hour of reading or watching, spend 3 hours building, solving, or running labs
- [ ] Log hours in `docs/log.md` at the end of each session
- [ ] No new chapter until the previous one has working code or a written lab report

### 2. Git Branch Hygiene

- [ ] `main` is always green and never receives direct commits
- [ ] One branch per deliverable: `phase-N/short-description`
- [ ] Small commits with imperative messages; squash-merge via PR after checks pass
- [ ] Delete branches after merge

### 3. Quality Gates

- [ ] `mypy --strict src/` passes before every PR
- [ ] `pytest --cov=src --cov-fail-under=80` passes
- [ ] `ruff check .` and `ruff format --check .` pass

### 4. Branch-Specific Rules

- [ ] Every solved problem has type hints, a complexity note in the docstring, and an edge-case test
- [ ] Attempt each problem for 20 to 30 minutes before reading any solution
- [ ] Log failures in `docs/dsa_log.md` and re-solve on days 3, 7, and 21
- [ ] Never paste a solution you cannot rewrite from memory the next day
- [ ] Test algorithms against a brute-force version on random small inputs

## Exit Criteria

- [ ] Solve most unseen LeetCode mediums in under 25 minutes
- [ ] Identify the pattern of a new problem within 3 minutes and justify it
- [ ] Prove the correctness and complexity of a greedy or DP solution
- [ ] Implement a segment tree and a Dijkstra with a heap without references
