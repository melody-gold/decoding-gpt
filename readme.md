(copy of `syllabus.pdf`)

|                 |                                                                                                   |
| :-------------- | :------------------------------------------------------------------------------------------------ |
| Course Code     | MATH 598B                                                                                         |
| Meeting Times   | 3:30pm-4:45pm, Tuesdays/Thursdays                                                                 |
| Location        | 211 Engineering Hall                                                                              |
| Instructors     | [Michael Ivanitskiy](https://mivanit.github.io), [Samy Wu Fung](https://swufung.github.io)        |
| Contact         | [`mivanits@mines.edu`](mailto:mivanits@mines.edu)                                                 |
| Office location | 269 Chauvenet Hall or Zoom by request                                                             |
| Office hours    | Time TBD, poll here: [`when2meet.com/?34348969-rJBxc`](https://www.when2meet.com/?34348969-rJBxc) |
| materials       | [`github.com/mines-opt-ml/decoding-gpt`](https://github.com/mines-opt-ml/decoding-gpt)            |
| website         | [`miv.name/decoding-gpt`](https://miv.name/decoding-gpt)                                          |


# Course Description

Since the public release of GPT-3 in 2020, Large Language Models (LLMs) have made rapid progress across a wide variety of tasks previously thought impossible. However, the internal mechanisms by which these models are capable of performing such tasks is not understood. A large fraction of machine learning researchers believe that there are significant risks from training and deploying such models, ranging from mass unemployment and societal harms due to misinformation, to existential risks due to misaligned AI systems. This course will explore the mathematical foundations of Transformer networks, the issues that come with trying to impart human values onto such systems, and foundations of interpretability and alignment research.


# Learning outcomes

Over the duration of the course, students will gain:

1. A solid understanding of the mechanics of transformer neural networks
2. Practical experience with implementing, training, and deploying LLMs for simple tasks
3. Understanding of the fundamentals of the AI alignment problem, present and future risks and harms, and a broad overview of the current state of the field
4. Familiarity with current results and techniques in interpretability research for LLMs


# Prerequisites

- Linear Algebra: Students should have a strong grasp of linear algebra, including matrix multiplication, vector spaces, matrix decompositions, and eigenvalues/eigenvectors.
- Machine Learning: Students should be familiar with basic Deep Neural Networks and stochastic gradient descent via backpropagation.
- Software: Students should be very comfortable writing software in python. Familiarity with setting up virtual environments, dependency management, and version control via git is recommended. *Experience with [PyTorch](https://pytorch.org) or another deep learning framework is highly recommended.*
- Research Skills: Students should be comfortable finding and reading relevant papers in depth. How you read papers, whether you take notes, etc. is up to you, but you should be able to understand novel material from a paper in depth and be able to explain it to others.

# Course Materials

This field moves too quickly for there to currently be an up-to-date textbook. Below are provided some useful introductory materials which we will be going over in part. Reading or at least skimming some these before the start of the course is recommended -- they are listed in a rough order of priority, but feel free to skip around. We will also be reading a wide variety of papers throughout the course, and you will be expected to find interesting and useful ones.

- **(START HERE)** [3Blue1Brown Series on Neural Networks and Language Models](https://www.youtube.com/watch?v=aircAruvnKk&list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi). An excellent series of lectures on neural networks leading up to Large Language Models. This series will be required viewing as a complement to the course material.
- [Stanford's CS324 course on Large Language Models](https://stanford-cs324.github.io/winter2022/)
- [The Illustrated GPT-2](https://jalammar.github.io/illustrated-gpt2/) by Jay Alammar, along with other blog posts in the series. Introduces the basics of attention heads, transformers, and autoregressive GPT-style models.
- Andrej Karpathy's [`nanogpt` implementation](https://github.com/karpathy/nanoGPT). A simple and minimal implementation of a GPT architecture.
- [Mechanistic Interpretability Quickstart Guide](https://www.neelnanda.io/mechanistic-interpretability/quickstart) by Neel Nanda. A compressed guide on how to get started doing interpretability research, with many useful links (follow them!). The [prereqs](https://www.neelnanda.io/mechanistic-interpretability/prereqs) are also useful.
- [The Transformer Circuits Thread](https://transformer-circuits.pub/2021/framework/index.html) by Nelson Elhage, Neel Nanda, Catherine Olsson, Chris Olah, and many others. Series of posts on some of the top results in transformer interpretability research.
- [AGI safety from first principles](https://www.alignmentforum.org/s/mzgtmmTKKn5MuCzFJ). Standard introduction for why AI systems might pose catastrophic risks, and overview of the kinds of work that need to be done to mitigate them. Of particular importance is [post 4 (Alignment)](https://www.alignmentforum.org/s/mzgtmmTKKn5MuCzFJ/p/PvA2gFMAaHCHfMXrw).
- [Risks from Learned Optimization in Advanced Machine Learning Systems](https://arxiv.org/abs/1906.01820) by Evan Hubinger et al. A paper on the risks of training AI systems to optimize for a particular objective, and the potential for such systems to become misaligned -- defines the inner alignment problem more formally.
- [Maxime Labonne's LLM course](https://github.com/mlabonne/llm-course/tree/main). A hands-on set of notebooks and resources on the more practical aspects of implementing, training, and using transformers.


# Evaluation

- **Homeworks (40%)** Short homeworks/mini projects will be assigned periodically, and will be due at the beginning of class on the due date.
- **Final Project: (50%)** Students (optionally working in groups) will select a research topic related to the course material, design and perform novel experiments, and write a report on their findings. Example topics will be provided, but topic selection is flexible, as long as it relates to alignment or interpretability for ML systems.
- **Class participation (10%):** Students are expected to attend course lectures, participate in discussions, and ask questions. Allowances for absences will be made.

# Tenative Course Outline

- Background
	- neural networks
	- autodiff, backprop, and optimization theory
	- other neural network architectures
	- language modeling
	- basic interp: linear probes
- Attention Heads & the Transformer architecture
	- attention heads
	- positional encodings, causal attention
	- transformers
- Interpretability
	- intro to interpretability
	- superposition and polysemanticity
	- linear probes
	- causal ablations
	- sparse autoencoders
	- parameter based interpretability
- Alignment
	- the AI Alignment problem
	- AI safety, ethics, and policy