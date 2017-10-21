# BlackJack
Plays a simple version of the casino game of blackjack; for 1 - 7 players

Interface Classes
Game

Implementation Classes
Card
  Each Card has its own rank and suit with status faceup or facedown. 
Hand
  Has a vector of Card pointer. Gets hand total value, intelligently treats aces as 1 or 11.
GenericPlayer
  Virtual Class derived from Card. Decide if the player has busted.
Player
  Derived from GenericPlayer. Decide if the player wants another hit. Decide the player wins, loses or pushes.
House
  Derived from GenericPlayer. Decide if house is hitting. Flips over first card when necessary.
Deck
  Derived from Card. Create a standard deck of 52 cards. Shuffle cards. Deal one card to a hand and give additional cards to a generic       player.
