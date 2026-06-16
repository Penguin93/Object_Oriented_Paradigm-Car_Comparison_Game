# Data Selection and Game Attributes

## Attributes
Price, Year, Power, Range, Odometer, Air Pollution Rating
## Ranking
Air Pollution Rating, Year, Odometer, Price, Range, Power
## Why each attribute was chosen
- Price was chosen as a standard attribute that would give a rough estimate of what the stats of the car would look like.
- Year was chosen as a secondary standard attribute that provides a more accurate estimate of what the Odometer and Price look like.
- Power was chosen as it is important in determining how well a car handles different types of terrain.
- Range was chosen as it provides a good estimate for what the fuel capacity and consumption for a car looks like.
- Odometer was chosen as it provides information for how long a car has been used and whether the quality of the car is good for its age.
- Air Pollution Rating was chosen to promote environmentally friendly cars and to raise awareness of how cars impact the environment.

## What makes each attribute fair or unfair in gameplay
- Price is a fair attribute as each car can vary wildly depending on several factors, and price generally correlates with how high quality a car is.
- Year is a fair attribute as usually correlates with the price and odometer of a car.
- Power is a fair attribute as cars typically have higher power depending on the type of car.
- Range is a fair attribute as it is usually dependent on the type of car and the quality of it. 
- Odometer is a fair attribute as it usually correlates to the car being older and cheaper, providing a high-rating stat for cars that may have few good stats.
- Air Pollution Rating is a fair attribute for allowing more environmentally friendly cars that might have lower stats to have a good chance in winning. Electric cars are also considered, although this stat might be unfair in favour of them as their air pollution rating is high due to the fact that they don't produce carbon emissions.

# Class Design

## Car
- Attributes: Price, Year, Power, Range, Odometer, Air Pollution Rating
- Methods: Pass attributes to Card
- Role in the system: The Car class stores all of the attributes of the car and keeps it separate from other classes as to not be accessed or changed directly.
## Card
- Attributes: Car
- Methods: Inherit attributes from Car
- Role in the system: The Card class displays the attributes of the Car class without allowing the attributes to be changed.
## Deck
- Attributes: Number of cards
- Methods: Shuffle deck, Deal cards
- Role in the system: The Deck class contains all of the cards and deals them to players when the game begins.
## Player
- Attributes: Name, Hand, Score
- Methods: Select attribute, Play card, Receive card
- Role in the system: The Player class handles all interactions that a player can do. It contains a player's name and their hand of cards.
## Game
- Attributes: Number of players, Deck, Number of rounds
- Methods: Start game, End game, Start round, End round, Determine winner of a round, Determine if a round ends in a draw, Determine winner of a game
- Role in the system: The Game class handles all of the interactions that can happen that allow the game to progress. It also handles any complications of a draw.

# Class Diagram



# Game Mechanics Design

## How the game works
- How a round is played: A round is played by a player playing a card and selecting an attribute. All other players play their card after the attribute is selected. The round ends once a winner is determined.
- How attributes are selected: The attribute of the round is selected by the player that won the previous round (On the first round, the attribute is selected by the player to the left of the dealer). The player selects an attribute by looking at their card and saying the attribute they want to select out loud.
- How winners are determined: A winner is determined by identifying the value of the selected attribute on each player's card. The player that played the card with the highest value of the selected attribute is considered the winner of the round.
- What happens in a draw: In the event of a draw, all cards played are stacked together and put to the side in a separate deck. These cards are then given to the player who wins the next round. If a draw happens again, all played cards get added to the deck. Repeat this process until a player wins a round.
- How the game ends: The game can end in two ways. The first way is once one player collects every card from every other player and is determined the winner of the game. The second way is once a predetermined number of rounds are played. The player with the most amount of cards at the end of the game is determined the winner.
## Game Balance
This game is balanced so that everyone has a chance of winning no matter what card they get. Some cards are more powerful than others, but every card has at least one high rating attribute and one low rating attribute.
## Unfair Advantage and how to fix it

## Modelled Structure Chart

# Interface and Card Design

## Card Design

## Game Interface Sketch


# Social, Ethical and Legal Implications

## Individual Impact

## Social Impact

## Environmental Impact

## Legal Considerations
