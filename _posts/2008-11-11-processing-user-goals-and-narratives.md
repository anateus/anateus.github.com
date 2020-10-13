---
permalink: /processing-user-goals-and-narratives/index.html
layout: post
title: Processing User Goals and Narratives
published: true
categories: []
---
In order to model a strategy to reach a goal, we need to parse some user input.

A goal is a particular frame with particular arguments. Each step in a strategy is---in fact---also a goal! Some goals are stubs, certainly.

This feature means that the system understands the underlying details better and better. If once <code>"make a salad"</code> is specified as a step in <code>"make a dinner"</code>, and later <code>"make a salad"</code> is narrated, next time <code>"make a dinner"</code> is undertaken, the details of salad-making can be taken into account.

So, how does one undertake processing a narrative?

Each sentence is examined separately. It is an underlying assumption of the system that sentences will be kept simple. So, the goal is one statement, and each sentence in the narrative is a statement.

I am adopting the method described in <a href="http://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.3.3085">"A Maximum Entropy Approach to FrameNet Tagging" (2008) by Michael Fleischman and Eduard Hovy</a>.

According to that model, the MaxEnt classifier (I'll be using an <a href="http://nltk.org">NLTK </a>impementation) will take these features: 
<ul>
	<li>Phrase type: PP, NP, etc.</li>
	<li>Voice</li>
	<li>Position: position in the sentence</li>
	<li>Grammatical function: external argument, object argument, etc.</li>
	<li>Head word: the verb in question</li>
</ul>

And decide what each word in the sentence is what frame element (Agent, Cause, etc.)

In addition to those features, an n-gram model may be applied, wherein the each subsequent word processed will be supplied the classification of some of the previous words, since once one word is classified as an Agent, another one is unlikely to also be one.

So, a user tells a simple story, and what do we get? We get a frame tagged with the head word. That is, a Motion frame, for example, would also include the particular verb lemma:
<ul>
<i>The boy walked to school</i>
	<li>Theme: "the boy"</li>
	<li>Direction: "to"</li>
	<li>Goal: "school"</li>
	<li>Head: "WALK"</li>
</ul>

The space of strategies is basically a graph of frames. As each frame gets defined in terms of possible subsequent frames, a <a href="http://en.wikipedia.org/wiki/Hidden_markov_model">Hidden Markov Model</a> of narratives is generated.

Then, a wide variety of techniques is available for leveraging HMMs to get us better strategies!
