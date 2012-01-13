---
date: 2012-01-13 13:09 PM
title: Coding is Writing
source: 
layout: post
---

Coding is writing. It's very functional writing, so it's easy to forget
that it's a written art and think of it as distilled digital action.
Really, for most people that's the right approach to take. It's
impossible to appreciate a novel or an essay without reading it for
yourself, but we all use software that we don't read, and in many cases
can't ever read even if we wanted to. But for a programmer, you can
write better programs with fewer bugs if you remember that you are not
just an engineer, but a writer as well.

In my experience, writers tend to have very clear ideas on how to
improve one's writing, and coders often have no idea how to improve
one's code. Perhaps that's because writing is an ancient art that has
been taught for thousands of years and computer programs are essentially
brand new to human history. Or perhaps it's because everyone reads more
or less constantly as a participant in modern society, but programmers
rarely read other people's code for any reason other than to modify or
fix it. Certainly it isn't common to read a piece of code because
it's widely regarded as well-written code whose style should be
emulated. Regardless of the reason, we programmers can learn a lot from
the guidelines and techniques that writers use to improve their writing.

### Show, Don't Tell

Of all the well-worn phrases used in English classes and writers'
workshops, "show, don't tell" is probably the most popular. A
well-written story pulls you in, and the force of the plot and
characters sweeps you effortlessly through page after page. A
poorly-written story plods along, laboriously explaining things that
should be inferred from the action and forcing the reader to slog
through page after page of unneeded exposition. In a good story,
exposition is only used when it is needed to provide context and
clarity to the story.

I think of exposition in stories as being like comments in a program. A
well-written program can be mostly understood through its structure and
the quality of its names for functions and variables. Reading through
the code should give you a strong sense of its purpose without the need
to resort to comments. That is not to say that good code has minimal
comments. Rather, good code uses comments only to good purpose: to
illuminate algorithmic choices and provide context and usage scenarios
and warn of possible failure modes. Bad code sometimes "over-tells" by
pedantically commenting every third line with redundant information that
insults the intelligence of the reader. On the other extreme, it may
omit comments altogether, leaving the reader to wonder about the
intended use of functions with unclear preconditions, postconditions,
and side-effects.

### Use a Consistent Style

Here, there is a very clear analogy. Many publications and organizations
have their own style guides governing issues that writers can reasonably
differ on. The [Chicago Manual of Style][], the [New York Times][], and the
[Associated Press][] are among the most prominent examples. They differ
on many points, but they're all perfectly readable and they cut down on
arguments about minor points of grammar and punctuation that aren't
particularly worth arguing about.

Similarly, many companies maintain coding style guides that prescribe
standards for indentation, brace placement, variable naming, file
structure, and so on. One very thorough example (which I like in most
respects) is the [Google C++ style guide][]. Programmers will never stop
arguing about code formatting, but it's far worse to deal with an
inconsistently formatted codebase than it is to deal with one that
doesn't use your favorite convention. The style rules for programmers
are essentially the same as the rules for writers: If you're working
with an established codebase, then conform to its style. If you're on
your own, then pick what you like, but stay consistent.

### Read, Then Read Some More

Here is where programmers fall short compared to writers. Great writ`ers
read thousands upon thousands of pages of prose en route to becoming
great (or even good) writers. They read much more material than they
could write in a lifetime. It's not feasible for a programmer to read
that much code, but most programmers only read their own work, code
directly related to their own work, and snippets that illustrate some
technique or API use that they want to integrate into their own code.

Writers and coders share a common experience of looking back on one's
own work and being embarrassed by its poor quality. If you're always
writing, whether its prose or programs, you should always be getting
better, so this phenomenon isn't surprising. However, we programmers
could dramatically speed the process up if we were more well-read in
code. Part of the problem is that there are established great works of
literature and non-fiction that aspiring writers can look to, but there
is no clear consensus on what codebases are are the best, or even what
the criteria are for a great codebase.

### Constantly Refine and Improve

There is an understanding among writers that good writing comes from
painstaking revision and editing. Hemingway said *GET THIS QUOTE*
something about throwing away most of his work. Often students don't
just turn in an essay and get a grade, they turn in a first draft and
incorporate the suggested revisions into their final essay. If a student
turns in a poor essay, it tends to come back covered in red ink, so
there is no shortage of information on what is going wrong and how to go
about fixing it.

I've seen some acknowledgement of this principle in the world of
software development, mostly from people suggesting that you should
build the first version of any complex system with the intent of
eventually throwing it away and rewriting it, because it will inevitably
be necessary at some point whether you like it or not. However, the idea
that functionally correct code may still be in need of significant
improvement is mostly absent. There are often practical reasons to write
quick and dirty code, but if quick and dirty is the only kind of code
you know how to write, you are severely limiting yourself. It's rare to
look over properly functioning code to try and determine how it could be
improved (unless it has a serious performance problem) because of the
possibility of introducing new bugs, but this process is essential to
the development of a good programmer.

### Write Without Ego

Developing a difficult skill requires a certain humility. You have to
admit that your work could be better, that other people can see flaws in
it that aren't apparent to you, and that by listening to them you can
improve. Then you have to listen to people criticize your work, and even
when they're trying to be diplomatic and sensitive, it usually feels like
they're attacking you directly and not just offering gentle suggestions
for improving your work. Taking this feedback and using it to improve
your work requires you to submerge your ego.

Writers always develop this skill, or else they wash out of writing.
It's impossible to seriously pursue writing without getting tons of
feedback, whether in an academic setting or in the real world. They
eventually gain a sense of when to take advice and when to ignore it,
and they gain a sense of their own strong and weak points as writers.

For programmers, this skill is much more rare. There seems to be little
effort made toward developing it through the equivalent of writers'
workshops or intensive editing sessions. Code review has fortunately
become more common, but often it is primarily focused on functional
correctness and adherence to the relevant style guide (for good
reasons), and questions of elegance, clarity, and conciseness are pushed
to the side. Writing without ego develops a programmer's skills
much more quickly, and allows the programmer to work better on a team.
It may even be a more valuable skill for a programmer than for a writer,
even though it is emphasized much less in the programming community.

[Chicago Manual of Style]:
[New York Times]:
[Associated Press]:
[Google C++ style guide]:

