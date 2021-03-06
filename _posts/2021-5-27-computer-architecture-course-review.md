---
layout: post
title: I have watched Computer Architecture course by ETHZ. Here is what I think about it
---

![preview]({{ site.baseurl }}/images/computer-architecture-review-preview.png)

Hi! This is the second post in my improvised series "I learned X and what I think about it". I intentionally cover good learning resources here, as I am convinced that knowing where to learn something is much better than knowing where not to learn something. So, this time we will discuss [Digital Design and Computer Architecture course](https://www.youtube.com/watch?v=AJBmIaUneB0&list=PL5Q2soXY2Zi_FRrloMa2fUYWPGiZUBQo2) lectured by professor [Onur Mutlu](http://people.inf.ethz.ch/omutlu/).

## What will be discussed and what won't

In this post I plan to talk about pros and cons of ETHZ CA course and give a brief explanation of what is covered there. So the targeted audience of this article are the software engineers, who want to learn computer architecture by their own, but who are not certain where to start. It is worth mentioning that I have my own opinion on university vs self-taught (online) education, but I am going to leave this topic for my another blogpost. 

## What does ETHZ Computer Architecture course cover?

![meme]({{ site.baseurl }}/images/meltdown-spectre-meme.png)

The roadmap of the course is pretty usual and follows most of the popular computer architecture books. It starts from the ground goes up, bringing new abstractions based on what was covered before. Such course structure is really good for students, as the process of studying is more like "inventing new technologies using existing knowledge received from older lectures" and not like "revealing how black-box technologies work, going deeper and deeper into them". Starting from the concept of transistor, the course builds up the understanding of logic gates, combinational and sequential logic, ALUs & registers and so on. To my surprise, it also covers some not mainstream, but quite interesting topics, such as systolic arrays. So for those who are already interested, here is a full list of key concepts which are discussed in the lectures (original order):

- Computer architecture, its field and architectures overview: CPUs, FPGAs, GPUs, TPUs

- Design goals, common constraints, Row-Hammer attack

- Combinational and sequential logic

- Hardware Description Languages and Verilog

- Timing and verification

- Von Neumann Model, Instruction Set Architecture, LC-3 and MIPS architectures

- Microarchitecture

- Pipelining and its issues

- Out-of-Order execution, Tomasulo algorithm

- DataFlow & load/store handling in OoO architecture

- Dataflow and superscalar execution

- Branch prediction

- VLIW and systolic arrays
- Fine-grained multithreading and SIMD Processors

- Graphics Processing Units and GPU Programming

- Memory organization: technologies, hierarchies, caches

- Cache issues and multiprocessor cache designs

- Virtual memory

## What I especially liked

![tomasulo-algorithm]({{ site.baseurl }}/images/tomasulo-algorithm.png)

when I started the course, I already had a superficial knowledge of most of its concepts, but that was definitely not enough. This was the main reason why I started watching the lectures in the first place.  Now, comparing me before watching the course and after finishing it, I can certainly say that I learned a lot. My huge respect to professor Multu - pipelining and Out-of-Order execution (including Tomasulo algorithm) were explained accessibly and really well. Caches were also covered in great detail, with parallels in design of virtual memory. I also have learned new design concepts, like VLIW and systolic arrays, which to my regret, I did not know before. I really liked the course idea of questioning every new introduced concept, showing it pros and cons and comparing it to alternatives. The key here is that there is no best design decision - every idea has some tradeoffs that computer architect make when designing a system. Such skeptical look encourages students to think more and analyze stuff, not simply memorize that "this is good" and "this is bad".

## What can be done better

![warp-scheduling]({{ site.baseurl }}/images/warp-scheduling.png)

As a graphics developer, one of my aims was to learn GPU architecture. And yes, it was covered in the lectures, but not so deeply as I would like. Certainly that was because the course aims to cover a wide range of topics and cannot go into every detail in each one, but it is needed to say that if you, like me,  want to study GPU architecture in depth, this course may be a good start, but will definitely be not enough. I also found sad that one of the most today's challenging topics, branch prediction, was explained quite fast, leaving modern standard prediction algorithms for self learning. Of course there is masters computer architecture course which focuses more deeply on exact concepts, but I wish that as much of them as possible might be learned from bachelors one.

## What's next

As I already said, one bachelor computer architecture course even from top-10 university is not enough to become a computer architect or a high educated C++ developer. The learning route of a professional never was a straight line and even I am not sure what to do next. Maybe I will watch [ETHZ CA master course](https://www.youtube.com/watch?v=c3mPdZA-Fmc&list=PL5Q2soXY2Zi9xidyIgBxUz7xRPS-wisBN&index=1) in the future (luckily it is also available on youtube). Maybe I will finally read [Structured Computer Organization By Tanenbaum](https://www.amazon.com/Structured-Computer-Organization-Andrew-Tanenbaum/dp/0132916525) which has been dusting on my shelf for a year. Maybe papers from Nvidia and AMD will be enough, who knows:)

Anyway, I am really glad that there are such good people like prof. Mutlu, who allow us to receive high-quality education for free. Universities will not lose any of their students if their lectures are available online for free, and their reputation will only increase, as more and more people will know the how high is the level of education they provide. So, do not forget to learn new technologies, share your knowledge and do good things for others! I hope this post was helpful for you, as usual if you have any questions and suggestions, or found a mistake in the article, feel free to [contact me](https://t.me/momodeve).