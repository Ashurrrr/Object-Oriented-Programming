# OOP Exercises Question 1
# Deck of Cards (Mr. Park's Answer)

```python
from random import shuffle as r_shuffle

class Card:
    def __init__(self, suit, value):
        self.suit = suit
        self.value = value

    def __str__(self):
        value = self.value # value variable exists in this method only.
        if self.value == 11:
            value = 'Jack'
        elif self.value == 12:
            value = 'Queen'
        elif self.value == 13:
            value = 'King'
        elif self.value == 14:
            value = 'Ace'
        return f'{value} of {self.suit}'

    def __repr__(self):
        return self.__str__()

class Deck:
    __SUITS = ['Spades', 'Hearts', 'Clubs', 'Diamonds']
    __VALUES = list(range(2,15))

    def __init__(self):
        self.deck = self.initialize_deck() # Setter method called: initialize_deck()

    def initialize_deck(self):
        result = []
        for suit in self.__SUITS:
            for value in self.__VALUES:
                result.append(Card(suit, value))
        return result
        # return [Card(suit, value) for suit in self.__SUITS for value in self.__VALUES]

    def shuffle(self):
        if self.deck:
            r_shuffle(self.deck)
            return True
        else:
            print('We have no cards in our deck.')
            return False

    def draw(self):
        if self.deck:
            return self.deck.pop()
        else:
            print('We have no cards in our deck.')
            return None
            ```
