# Design notebook for week ending November 16, 2014

## Description

This week I spent a lot of time discussing probability calculations in Magic: the Gathering. I spent a lot of time thinking about which of these calculations would be useful shortly to have implemented in my DSL. Overall, there are far too many potential computations that a user might want for me to implement them all from scratch.
Therefore, based on my critique feedback from last week, I have decided that the key will be making it as easy as possible to expand the Math language. For now, I'm still thinking that means making a grako syntax, because it is easy to add new grako rules, and their corresponding Python functions. However, I might also try to come up with some way of setting up a feature to allow users to define functions in their query file. 

For now, the result of this decision is that I have postponed creating a formal syntax on the query file for now. Queries will look sometthing like

```
For decks <list of decks>: 
	Given (<condition1>, <condition2>, ...) probability of <result>

Plot all output
```

Every query that we could come up with had this form, (with givens and a result), but we came up with a very large number of potential conditions and results for me to consider implementing.

On the Deck side of things, a formal syntax (in grako) is present in project/src/deck.grako. Grako takes grammars in roughly EBNF form, so it should be recognizable to anyone reading it. I also have an IR specified, as laid out at one point in project/documents/design_and_implementation.md.


## Questions

**What is the most pressing issue for your project? What design decision do
you need to make, what implementation issue are you trying to solve, or how
are you evaluating your design and implementation?**

The most pressing issue for me right now is to figure out the best way to create easily extensible grammars with semantics (for the Math language). However, in order to stay on the pace I set out in my plan, I might end up using a slightly less extensible system in order to finish before the end of this class.

**What questions do you have for your critique partners? How can they best help
you?**

Do you think that it is reasonable to expect users to edit a file containing a portion of the EBNF grammar, as well as adding Python functions for the conditions they add. By my understanding of how Grako works, I believe that it is possible to do this in an extensible manner. Otherwise, do you know of any tools that might do this better?

Can you think of any questions you might have that are not of the form "Given _______ calculate the probability of _______" for any card game?

**How much time did you spend on the project this week? If you're working in a
team, how did you share the labor?**

I spent about 1.5 hours writing and responding to critiques.

I spent a large number of hours (3+, although possibly not as productive as they could have been) thinking about and discussing probability calculation in Magic: the Gathering.

I spent about 3 hours writing up the formal grammar for Deck, and coming up with some sample files (in project/samples).

I spent about 1.5 hours writing up the design and implementation.

I spent about 1 hour on this notebook entry.

## Post-critique summary

## Post-critique reflection
