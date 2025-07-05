---
layout: post
title: Second-order Inquiries on Statistics
date: 2024-11-09
tags: Philosophy Statistics
categories: Thoughts
citation: true
---

## What Is Statistics, Really?[^1]

Wikipedia defines statistics as "the discipline that concerns the collection, organization, analysis, interpretation, and presentation of data". However, this definition is too operational and insufficiently general. If I were to define statistics, I would call it **the study of inductive reasoning**.

Statistics occupies a unique position; it is neither like mathematics and logic, which fall under the category of [formalsciences](https://en.wikipedia.org/wiki/Formal_science), deriving new truths from existing true propositions through deductive reasoning, nor is it like the natural sciences, such as physics or chemistry, which use inductive reasoning to derive knowledge about the world from observations. From my perspective, statistics tries to answer a fundamental epistemological question: how can we preserve the validity of inductive reasoning? Statistics tries to find optimal “inductive strategies” with desirable "deductive qualities", and that’s why we attach importance to aspects like unbiasedness, invariance, and asymptotic normality.

The fundamental flaw of inductive reasoning is that it is not truth-preserving. As David Hume illustrated, no matter how many black crows we observe, we can never conclusively claim that all crows are black; induction cannot guarantee truth beyond what we have seen. However, astonishingly, statistics lets us make certain statements like “under some assumptions, we believe all crows are black with over 95% confidence.” From incomplete and uncertain data, we manage to arrive at conclusions that are rigorously defensible—-a philosophically extraordinary feat that reveals the significance of statistical reasoning

Of course, this assurance comes at a price: statistical statements are always weaker than the original propositions. Universal claims become probabilistic, and exact statements become approximate. Yet by accepting this trade-off, we transform inexpressible questions into expressible ones, and metaphysical problems into mathematical ones.

Moreover, statistical inference always relies on an unverifiable assumption that the data originates from "some underlying probability distribution." Reflecting on this assumption leads to another interesting question in philosophy of science: the question of realism versus instrumentalism. 

## Statistical Models: Reality or Mere Tools?

In the philosophy of science, there is a long-standing debate between realism and instrumentalism. Realism holds that scientific theories should reflect reality, while instrumentalism requires only that they provide explanations and predictions.

For example, is gravity an actual force present in the objective world, or is it just a "model" physicists use to describe our world? Most people lean towards the former, though proving this philosophically far from straightforward. In contrast, many adopt an instrumentalist stance on quantum theory, caring little about whether quantum states are "physical realities" and treating the theory purely as a "predictive tool"--sumed up by the famous phrase, "shut up and calculate."

However, in statistics, few concern themselves with whether models represent any "physical reality.", and among those who do, almost none hold a realist stance. Some may see normal distributions or linear models as the "real-world mechanisms" generating data. But no one believes random forests or neural networks "exist" in any ontological sense; they are simply tools for prediction. 

More strikingly, identical mathematical structures often emerge in statistics from entirely different views on reality. For example, principal component analysis (PCA) can arise from maximizing data variance, minimizing distances to a linear subspace; or even from game-theoretic derivations. Philosophically, what does it mean when the same structure emerges from disparate perspectives? 

Unlike the natural sciences, statistics is highly instrumentalist, and this abandonment of realism has led to models with remarkable predictive power, such as deep learning. George Box’s famous saying, "All models are wrong, but some are useful," perfectly encapsulates this instrumentalist mindset.

## Concluding Remarks

Our discussion reveals how closely statistics is intertwined with epistemology. By employing mathematics and models, statistics offers a framework for making sense of an objective world that we can never fully grasp with certainty. This profound link reminds us that statistics is not merely a technical tool, but an essential part of our ongoing quest to understand the limits of human knowledge.


[^1]: My mind has been greatly influenced by [Ludwig Wittgenstein](https://en.wikipedia.org/wiki/Ludwig_Wittgenstein) and Analytical Philosophy. This article discusses my thought about statistics from a philosophical perspective. Actually, it is the philosophical significance of statistics that attracts me to this field. Also, [here](https://www.bilibili.com/video/BV1TD421g7Y6/?spm_id_from=333.999.0.0&vd_source=122f65726f0fe678830e7adff2d7c3ff) is a talk (in Chinese) I gave to the junior students at SUSTech about why I chose to study statistics.



