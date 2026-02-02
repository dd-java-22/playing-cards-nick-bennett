# Card trick

# Definitions

- `deck`: `Deck`, initially containg an equal number of black and red `Card` references. A `Deck may` be shuffled, and cards can be dealt from it, until it is empty; each `Card` has a color.
- `blackPile`: `List` of `Card`, initially empty.
- `redPile`: `List` of `Card`, initially empty.
- `random(n)`: `Integer`, selected at random, with equal likelihood, from {0, 1, ..., (n - 1)}.

# Steps

1. Shuffle `deck`, using an appropriate method (e.g., Fisher-Yates), with the `random` function as a source of randomness.

2. Repeat until `deck` is empty:

    1. `selector`: `Card` &larr; next `Card` dealt from `deck`.

    2. If color of `selector` is black:
   
        - Add next `Card` drawn from `deck` to `blackPile`.

        Otherwise:
   
        - Add next `Card` drawn from `deck` to `redPile`.

3. Verify that: count of black `Card` values in `blackPile` = count of red `Card` values in `redPile`.