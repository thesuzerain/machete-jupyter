# Machete-analysis

A mostly experimental collection of processing + analyzing scripts for extracting metadata from TTRPG data.

For eventual use in [Machete](https://www.github.com/thesuzerain/machete).

## Motivation

When preparing to play a tabletop role-playing game like Dungeons and Dragons, or Pathfinder, the *game master* (read: organizer, or game designer) often finds themselves pouring over endless books and tables to craft the perfect shop or combat encounter. 

- Is a `young red dragon` the right level for my party and players? What about a `goblin priestess`?

- How much loot should I give for beating a `behir`?

Sometimes, the questions are a little bit harder to answer mathematically. for example:

- A red dragon is an enemy that usually is difficult to fight for melee combatants. My party are mostly melee characters, and one player has a fire weakness. How much does this impact my fight?

- I have an extra 50 gp worth of loot to give to the party for winning the fight against the `Blood Hag`. Which item should I give that shores up some of the the weaknesses in their party?

## The idea

We want to infer metadata from TTRPG data tables to help answer these difficult questions. 

- We can infer semantic tags from names and description to find connections that aren't explicitly defined: which monsters are associated with goblins? which weapons are associated with starlight? 

- We can infer item relevance to a given campaign (a ship being more relevant to a pirate campaign than a desert one) or to a certain class (a sword being more useful to a fighter than a wizard- or more subtly, is a scroll more important for a wizard or sorcerer?)




### Alternatives

An easy use case for these kind of questions could be ChatGPT, or another similar LLM. However, this comes with notable drawbacks.

- LLMs are excellent at deciphering information from natural language. However, they struggle on the next stage: consistent calculations and formulaic predictions. For games like Pathfinder, where a lot of the numbers are heavily formula-based, this becomes a hurdle.

- LLMs can have a comparatively large energy expenditure (and for APIs, a small but non-negligible cost expenditure) for what should be easily calculable problems. This is exacerbated if a generator is used over and over again if the results are not as desired. 

    - There are lots of problems that are difficult to solve without LLMs or genAI. However, for this problem, it's overkill.
