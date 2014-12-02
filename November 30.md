# Design notebook for week ending November 30, 2014

## Description

Deck is bascally done. The semantics are in project/src/semantics.py, which
still doesn't fully work, and hasn't been thrown in with the grako parser.
However, cleaning up the last TODOs and adding it to grako should be less than
an hour of work at this point.

I got to do cool stuff with the product library to effectively create a number
of for loops to be defined at runtime. I thought it was an interesting problem,
you can see the results in the card_rule function in semantics.py

I also wrote up the preliminary evaluation document this week. Next week is
finish Deck, and hopefully get Math working, so that everything is at a point
of just needing to be cleaned up.


## Questions

**What is the most pressing issue for your project? What design decision do
you need to make, what implementation issue are you trying to solve, or how
are you evaluating your design and implementation?**

I just solved the runtime-defined number of for loops issure, so I'm not super
blocked on anything right now. Mostly, I just need to get Math working at this
point. I have a pretty good idea what it's going to look like, so it should be
possible to code it up and get it working in a single week, given that I now
have practice with grako. 

**What questions do you have for your critique partners? How can they best help
you?**

Take a look at the sample_decks file in project/samples/sample_decks.deck. See
if you understnad what's going on with how Deck works, and let me know if you
think there are any glaring feature holes in terms of defining a deck. Remember
that the cards don't need to have all of the information necessary to play a
game, they just need enough information to be able to fit any queries you might
make in the Math language.

**How much time did you spend on the project this week? If you're working in a
team, how did you share the labor?**

In total I spent about 7 hours on the project this week. That was ~1 hour on
the preliminary evaluation, and figuring out how my Math syntax would look,
along with 6 hours of writing Python code.

## Post-critique summary

## Post-critique reflection
