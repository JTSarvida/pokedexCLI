
# User Story

## Who is my User?

The User for this app would be Pokemon enthusiasts who enjoy playing the main games in the series. 

## What is the User's Pain Point?

The User is either new to the series, or is returning to the series after several generations. 
Both instances require a refresher on old Pokemon, as well as information on any new Pokemon that they haven't experienced yet.

## How do they use our solution to overcome this problem?

The User is playing their pokemon game and need some information in order to build their team for a certain battle. They go 
to our app, and type in the Pokemon's name. This will provide them with a quick snapshot of that pokemon, plus options to view other parts about them, ie move learnsets,
egg moves, etc.

# Choosing the Classes for this app

## Pokemon Class

While scraping the marriland national pokedex page, we as Users are searching for specific Pokemon. This Pokemon object will have these traits available for our snapshot:

1. Name
2. Type

We are then prompted if we want to learn more about the Pokemon, which will bring up the Pokemon's ability(s), Base Stats (HP, Attack, Defense, Sp. Atk, Sp. Def, Speed), and Level Up Moves

So Pokemon will have a total of 5 traits, 10 if we count all of the Base Stats.

## CLI Class

This class is essentially the Pokedex interface itself. It will introduce itself as the National Pokedex that features all 8 generations of Pokemon. It will then prompt you to ask about any specific pokemon. 
Once the User answers these prompts appropriately, the Snapshot of the pokemon shown above will be displayed, followed by a prompt asking if the User want's more info. If yes, the Pokedex will display the additional 3 traits 
mentioned above. Once this is done, the Pokedex will ask the user if it would like to look up another Pokemon. If yes, then it'll cycle through the beginning of the Pokedex prompts. If no, it will say goodbye and end the program.

## Scraper Class

This is the class that's responsible for scraping through Marriland's National Pokedex page. This website was selected as it provided easily identifiable classes for each aspect of the Pokemon I was looking to scrape for.
We will be starting off on the Marrilland's National Pokedex page, grabbing all the names and types of each pokemon spanning all 8 generations. We also scrape through each Pokemon's personal dex page, scraping for those 3 detailed
traits mentioned above.

