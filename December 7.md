# Design notebook for week ending December 7, 2014

## Description

Deck is done. That is a great milestone. It's been hovering at almost done for
what feels like the longest time, but now it's finally done. In order to see it
at work, navigate to the `src` directory in my project, and first run
```
grako deck.grako > g_deck.py
```
(Note: it must go to exactly g_deck.py, you cannot name the file anything different)

Then, you can run the command 
```
python parse_deck.py <deck-file-path>
```
to parse a deck, and see some output and some final statistics on the deck that
was parsed.  Some good decks for testing are `project/samples/bad_cards.deck`
which is a deck of playing cards with an extra 5 of clubs, and
`project/samples/legacy_burn.deck` which is an example of what a deck of Magic:
the Gathering cards might look like. (You can access these in the command above
as `../samples/<deck-name>`)

Also, I have a preliminary plan for my presentation, located in the
Presentation_Plan document in the root folder of my project.

Finally, I have a sketch grammar for the Math DSL, which is located in
project/samples/preliminary_math.txt. The goal is that over the course of this
week I can make that into EBNF and have it run some basic calculations, so that
my problem will be somewhat complete in that aspect as well. Plotting might
have to be reserved for the future.

My other task this week (aside from the final write-up and finishing Math) will
be to make a shell script to do all of the grako building for you, so that all
you have to do is something like
```
do_math.sh <math-file-path>
```
and it will make sure everything is compiled and ready, and then call the
appropriate python command to do the math you want. 


## Questions

**What is the most pressing issue for your project? What design decision do
you need to make, what implementation issue are you trying to solve, or how
are you evaluating your design and implementation?**

I need to get Math implemented and working. It seems like it might be a one-week
task now that I am more familiar with grako. This whole week is mostly going 
to be focused on that.

**What questions do you have for your critique partners? How can they best help
you?**

If you want to check out the sample decks and provide some feedback on those, 
that would be neat. However, what I'm most interested in this week are your 
thoughts on the sktech grammar I have for the math DSL in 
`project/samples/preliminary_math.txt`. Is there anything you think it's missing
based on our discussion in class? Is there anything that could be better? Is
there anything it should be able to do?


**How much time did you spend on the project this week? If you're working in a
team, how did you share the labor?**

This week only had about 5 hours outside of class, but it had extremely productive
class time compared to previous weeks, due to the prototype demo in class, and crunch
time kicking in to make me want to work on the other days.

## Post-critique summary

## Post-critique reflection
