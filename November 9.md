# Design notebook for week ending November 9, 2014

## Description

A note on this week: I slightly broke my laptop this week, (it's fixed now)
which that means that I have a lot of stuff written down on paper. It will go
up in the repo later in the week, but I don't have it up yet. I'll try to put
the key points to critique in this notebook entry.

This week I spent a lot of time thinking about the internal represenation I
wanted to use, along with the host language. I ended up deciding I want to try
to do everything in Python, because the SciPy library looks like it has a lot
of the plotting and math features I am interested in for the calculation DSL.

Python will also allow me to implement the internal representation of my decks
using a class hierarchy: Deck -> Card -> Trait. Dictionaries are very
convenient here, and Python does them well. I have an interface written up for
each of the three components that should allow the Math language to do its work
in very few lines of Python code after it has been parsed.

I also have a sketch grammar written for the syntax of the Deck DSL. The goal
in coming up with it was maximum simplicity, requiring very little more than
the minimum possible amount of text for a deck setup, so that they are quick to
jot down.

## Questions

**What is the most pressing issue for your project? What design decision do
you need to make, what implementation issue are you trying to solve, or how
are you evaluating your design and implementation?**

The main design I will be focusing on in this coming week is the syntax for the
Math DSL. This also means figuring out what requests will be able to be made in
the Math language. Originally, I expected to be limited by what was easy to
generate output for, but SciPy seems to have lots of good tools, so it's more
going to be what I can implement in this time frame. The goal will be to make
the language powerful, but also easy to remember so that I can come back to it
in the future and still understand/make new queries.

**What questions do you have for your critique partners? How can they best help
you?**

Do you know how to write parsers in Python? Are there combinators like there
are in Scala/Haskell? This is research I can do, but if you happen to know good
resources it would be great if you could share.

Also, can you think of calculations that you would really want done? (Think
along the lines of Magic, Hearthstone or any playing card game) I will try to
make the syntax so that if it doesn't include it immediately, then at least it
would be easy to expand to include the calculation in a simple manner.


**How much time did you spend on the project this week? If you're working in a
team, how did you share the labor?**

I spent about 4-5 hours thinking about IR, and scribbling things on various
sheets of paper, some of which got crumpled up and thown away (bad, I know, but
I was mad at them). There was also about two hours spent on critique-involved
activities.


## Post-critique summary

## Post-critique reflection
