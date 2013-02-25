---
layout: post
title: "Solving a Major Problem -- Bras"
date: 2013-02-24 21:59
comments: true
categories:
---

I like learning about other people's problems. I particular like learning about problems from people who have different problems than mine and one of the most common and persistent of those is the issue of bras. Many women told me about it and complaints were near universal and came from all quarters. I've specifically asked a lot of women about their experiences with bras to better understand and also did research on the state of the art of design, engineering and manufacturing of bras. This is something that affects women with breasts of all sizes--it isn't restricted to women with big breasts. I realized recently that although I'd love to work on this problem, without some help I can't do it. I'm not a domain expert in several of the fields required, though I've gone into some depth on the subject, so writing about it would perhaps inspire someone to either join me or take it up on their own.

*An important note:* It is common amongst engineers and programmers to wade into a new domain with a savior complex, "we'll fix this for you with our fresh perspective!". On a slightly different slant, a lot of women have experience [mansplaining](http://www.urbandictionary.com/define.php?term=Mansplain). I'm trying very explicitly to not be doing either of these. I'd like this to be an overview of what I've discovered and what I think is a good solution. I'm not swooping from above magically delivering bra salvation to the helpless female masses. I just haven't seen these ideas put together before and thought folks might be interested. Just wanted this to be clear.

## The Problem

Bras are required to perform these core functions:

1. Mold the breasts into the currently fashionable shape and thus look attractive when viewed under clothing
2. Look attractive when seen without other clothing covering them
3. Be supportive: allow for a wider range of vigorous activities than some women can easily accomplish without

In order to perform #1 and #2 bras are form-fitting so as to not be prominent under clothing. Form-fitting is best achieved with stretchy fabrics, which would make either #3 or #2 hard (sports bras for example sacrifice #2). Underwires were introduced to be able to move most of the difficult parts of providing support to a rigid elements made of plastic or metal. If a form-fitting item is not stretchy it will always be uncomfortable if it is not custom made. This is the core reason reason bras are so uncomfortable. It's the only clothing item of this sort I can think of that is commonly worn. Imagine briefs made from dress shirt fabric. That is not a pleasant thought.

Bra sizing is terrible. The cup size of a 32C and a 34C is of a different size even though it's designated as C. The way most companies design bras these days is that they a group of women that they used to measure and now usually perform 3D laser scans on called the *model pool*. Using the model pool they derive their band size to cup size function. This means that the particular function varies from manufacturer to manufacturer. So not only are the sizes themselves inconsistent between manufacturers the *steps* are also different since the sizing function would vary by their particular pool and how they segmented it. On top of this there are the core issues of breast asymmetry and placement: The vast majority of women's breasts are asymmetrical and the distance between the breasts varies a lot. These are not taken into account in the sizing and adjustment for them is minimal if available at all.

So, bras are uncomfortable and under the current model can't possibly be made comfortable. A less egregious but annoying aspect of the bra industry is that they subtly imply but never state that the bras might affect breast sagging (the technical term for which is *ptosis*). Repeated studies by the industry have shown this to not be the case (breasts will sag with age regardless of bra wear), so they never claim it outright but merely hint. Additionally, there are medical effects such as back pain and problems with the lymph nodes that result from imperfect fit.

This is a problem that ranks highly on both the scales of *pain* and *persistence*. This is a daily issue that causes many women a lot of suffering. It's a big deal.

## The Solution

We must be able to create a custom bra for each woman. My proposed method involves performing a 3D scan of the breasts from which a custom pattern is derived.

The state of 3D scanning as evidenced by products such as the Kinect or the [Leap](http://leapmotion.com/) is such that large and slow laser scanning equipment is no longer necessary. Small units can be built and placed inside changing rooms in existing stores or perhaps in some sort of booth.

Fundamentally, a bra is an item that applies certain force vectors to from a source shape to a target shape. Current design techniques in the industry treat the breasts as liquids filling a form. The form is anchored to a body and they perform simulations not very different from those involved in other structures such as bridges to ensure forces dissipate in optimal ways throughout the bra and through the body. This sort of analysis would still be necessary, but with a 3D scan of the breasts we can create an accurate model of the breasts. So one woman might need additional support in a particular angle while another who may share her exact band and cup size would not, merely due to the differences in shape and volume which are now available!

Advances in textile manufacturing also provide potentially interesting elements. Better weaving machines are able to construct fabrics with custom 3D structures so that things like the fabric's elasticity can vary throughout without varying the amounts of a different material. Manufacturing supply chains, and custom orders are increasingly more common, easy and cheap. We get the additional advantage of being able to respond to changing fashions in both the desired target shape and appearance more easily than traditional approaches.

So to get something like this done, one would need to be good at 3D scanning, the math required to do the tensor math for the breast shaping, the math for turning those force vectors into a pattern, the math and engineering required to optimize the patterns and the necessary textile manufacturing instructions, and the business connections to get the manufacturing done well and cheaply.

A custom bra is necessary. There's just no other way to fulfill all 3 core tasks. I'd love for someone to tackle this. Please do contact me with any thoughts you might have on this, it's more important than it might seem.