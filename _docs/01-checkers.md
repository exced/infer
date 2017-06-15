---
docid: checkers
title: "Infer : AI"
layout: docs
permalink: /docs/checkers.html
---



Infer.AI is a collection of program analyses which range from simple checks to sophisticated inter-procedural analysis.  
Infer.AI is so named because it is based on Abstract Interpretation. 

Current Infer.AI's which are in production include ThreadSafety, 
AnnotationReachability (e.g., can an allocation be reachef from a @PerformanceCritical method), and [immutable cast](docs/checkers-bug-types.html#CHECKERS_IMMUTABLE_CAST) for Java, as well as Static Initialization Order Fiasco for C++. 

The current checkers can be run by adding the option `-a checkers` to the analysis command as in this example:

```bash
infer run -a checkers -- javac Test.java
```

In addition, we are working on experimental AI's which target 
security properties (Quandary) and buffer overrusn (Inferbo). The infer commandline man page
(`infer --help`) tells how to run experimental AI's, or to select certain AI's and not others.

 