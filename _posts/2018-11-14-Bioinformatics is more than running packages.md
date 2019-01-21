---
layout:     post
title:      Bioinformatics is more than running packages
date:       2018-11-14
author:     Xuan
catalog:    true
tags: Comment
---

# Thinking about the algorithms in packages before running the code

With the development of the NGS field , now there are tons of
bioinformatics packages available for data analysis. There are a lot
package choices for each step of the NGS analysis. For example, tons of
short sequence alignment algorithms have been developed to meet the
requirements. There are also different statistical strategies to call
the significance of the differential gene expressions.

Novel researches and significant findings have been made possible
through those  NGS studies. And thanks to GUI based NGS analysis
software platforms like Galaxy and other commercial softwares, the NGS
data analysis become routine in labs. Also linux environment
configurations are becoming easier with the Anaconda or Biolinux OS,
which allows people to get used to UNIX system more easily.

From my personal experience with the NGS data analysis, it is routine to
derive some minor differences for the same set of dataset using
different package combinations, sometimes even the package versions made
slightly differences too. Take the Clip-Seq data analysis as an example,
the peak calling part is still a big problem in the field due to
non-specific interactions and background noise. eClip experiment solved
the background problem by introducing a blank input control in the
library preparation, but that comes with an expense of additional labor
and sequencing costs. The main questions raised from the Clip-seq versus the
RNA-seq seemed different, one is to identify the protein binding site and the
other for determination of the differentially expressed gene. In essence, Clip-Seq is not significantly different than RNA-Seq because identifying differential enriched binding elements versus differentially expressed genes stem from the RPKMs of the binding sites. Of course, there are also additional steps that considers the shape and distributions of the binding peaks for the Clip-Seq datasets, but their basic ideas are the same and understanding the algorithms and mathematics used in the packages will make marked differences in answering the biological questions.

