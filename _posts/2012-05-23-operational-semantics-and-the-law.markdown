---
date: 2012-05-23 22:45 PM
title: Operational Semantics and the Law
source: 
layout: post
---

Listening to this week's
[Hypercritical](http://5by5.tv/hypercritical/68), I was struck by links
between John Siracusa's discussion of the interpretation of laws and my
own memories of learning about the formal interpretation of computer
programs. Without interpretion, whether by judges, legislators, or law
enforcement, laws are just words on paper. It's only in the process of
interpretation that they acquire real-world significance, and often
there are multiple competing plausible ways of interpreting a given law.
While there is much debate between competing schools of legal
interpretation, Siracuse claimed that judges probably tend to make their
decisions for personal ideological reasons and rationalize a consistent
interpretive framework after the fact. I'm inclined to agree with him.

Still, it's worth thinking about what it would be like if laws always had a
clear and unambiguous real-world meaning, with no room for subjective
analysis. It would, I claim, be a lot like computer programming.
Computer programs, like laws, are just a collection of words, though
they're usually on a screen rather than paper. Programs can be
translated to actions in the real world by executing them on a computer,
much as laws can be translated to real-world actions by passing and
enforcing them on a population.

Computer programs have very strict rules about how the words on the page
are converted into changes in the state of the computer that they're run
on. The formalization of these rules are called [operational
semantics](http://en.wikipedia.org/wiki/Operational_semantics),
and they form a strict and logically consistent framework for reasoning
about what a program can and can't do. The process of actually reasoning
about programs is still incredibly difficult and incredibly tedious (I
remember spending the better part of a week of class time being spent on
proving that after executing the statement "x = 1", the variable x will
contain the value 1), but it's possible to make completely unambiguous
and objective statements about what a program *means*, as opposed to
just what it says.

In comparison, the law will always be a bit fuzzy, despite specialized
legal language that aims for precise and unambiguous meanings. I think
that people who spend a lot of time talking about the original intent of
lawmakers are wishing for a precise operational semantics for the law,
in which one could reliably answer any legal question just by asking its
writer what they intended (possibly using necromancy for our older
laws). Unfortunately, this desire ignores the complexities of lawmaking
in the real world. Laws don't have a single author, rather they are
written and passed by groups of interested parties who may not all have
the same goals or the same interpretation of the law. Even if it was
possible for a judge to summon up the lawmakers who passed a bill,
there's no reason to think that they would agree on how that bill should
be interpreted now.

Of course, even if we did have a precise operational semantics for the
law, I doubt it would help anything. Instead of arguing about original
intent, we'd be complaining about the rampant bugs in our laws.


