---
title: "BLAS-on-flash: An Efficient Alternative for Large Scale ML Training and Inference?"
collection: publications
permalink: /publication/blas-on-flash-nsdi
excerpt: 'Many large scale machine learning training and inference
tasks  are  memory-bound  rather  than  compute-bound.
That is, on large data sets, the working set of these al-
gorithms does not fit in memory for jobs that could run
overnight  on  a  few  multi-core  processors.   This  often
forces  an  expensive  redesign  of  the  algorithm  for  dis-
tributed platforms such as parameter servers and Spark.
We  propose  an  inexpensive  and  efficient  alternative
based on the observation that many ML tasks admit al-
gorithms  that  can  be  programmed  with  linear  algebra
subroutines.  A library that supports BLAS and sparse-
BLAS interface on large SSD-resident matrices can en-
able  multi-threaded  code  to  scale  to  industrial  scale
datasets on a single workstation.
We demonstrate that not only can such a library pro-
vide  near  in-memory  performance  for  BLAS,  but  can
also be used to write implementations of complex algo-
rithms such as eigensolvers that outperform in-memory
(ARPACK) and distributed (Spark) counterparts.
Existing  multi-threaded  in-memory  code  can  link  to
our library with minor changes and scale to hundreds of
gigabytes of training or inference data at near in-memory
processing  speeds.   We  demonstrate  this  with  two  in-
dustrial scale use cases arising in ranking and relevance
pipelines: training large scale topic models and inference
for extreme multi-label learning.
This suggests that our approach could be an efficient
alternative to expensive distributed
big-data
systems for
scaling up structurally complex machine learning tasks.'
date: 2019-02-26
venue: '16th USENIX Symposium on Networked Systems Design and Implementation (NSDI)'
paperurl: 'http://harsha-simhadri.org/pubs/nsdi19_final.pdf'
citation: 'Subramanya, Suhas Jayaram, et al. "BLAS-on-flash: An Efficient Alternative for Large Scale ML Training and Inference?." 16th USENIX Symposium on Networked Systems Design and Implementation (NSDI 19). USENIX Association.'
---