---
layout: post
title:  "Quantum Magic"
categories: quantum
date:   2018-11-27 21:45:24 -0800
series: "Exploring Quantum Computing"
excerpt: 
  A peek into the math that drives the magic of quantum computing.


something: else
---

{% include quantum_toc.html %}


# bits and qubits

## classical bits

Bits are very simple. Any given bit can only be one of two possible values. To match quantum computing notation, we will call those two values 
$$\langle0|$$ and $$\langle1|$$.

We can also look at a collection of bits. Nothing much special happens with a collection of bits. Suppose we have 4 bits. Then each bit independently can either be 
$$\langle0|$$ or $$\langle1$$.
If, for example, the third bit is
$$\langle1|$$
and the rest are 
$$\langle0|$$,
Then we write the collection as
$$\langle0010|$$.

This is all simple, and honestly not very exciting. But it will get more interesting when we venture into the quantum world.

## qubits
We’re going to use some weird notation, but that’s just because we’re introducing us to the quantum world.

A bit can either have the value $$\langle0|$$ or $$\langle1|$$. Mathematically, a qubit on the other hand is a  combination of the possible classical values. That is, a generic qubit is 
$$\langle\psi| = a\langle0| + b\langle1|$$
where 
$$a,b \in \mathbb{C}$$
and $$|a|^2+|b|^2 = 1$$. It is tempting to say that a qubit is between the two values, but it really is _both_ values at the same time.

Given a classical bit we can always know exactly which possible value it is. But this is where qubits start to get weird. Unless we prepared the qubit we don’t necessarily know what state it is in. What we can do though is _measure_ the qubit. Given a qubit 
$$\langle\psi|=a\langle0|+b\langle1|$$, if we _measure_ the qubit then it will “collapse” into either $$\langle0|$$ or $$\langle1|$$ with probabiltities $$|a|^2$$ and $$|b|^2$$ respectively.
