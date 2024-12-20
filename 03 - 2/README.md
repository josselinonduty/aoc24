# Day 3: Mull It Over

[https://adventofcode.com/2024/day/3](https://adventofcode.com/2024/day/3)

## Description

### Part Two

As you scan through the corrupted memory, you notice that some of the conditional statements are also still intact. If you handle some of the uncorrupted conditional statements in the program, you might be able to get an even more accurate result.

There are two new instructions you'll need to handle:

- The `do()` instruction _enables_ future `mul` instructions.
- The `don't()` instruction _disables_ future `mul` instructions.

Only the _most recent_ `do()` or `don't()` instruction applies. At the beginning of the program, `mul` instructions are _enabled_.

For example:

    xmul(2,4)&mul[3,7]!^don't()_mul(5,5)+mul(32,64](mul(11,8)undo()?mul(8,5))

This corrupted memory is similar to the example from before, but this time the `mul(5,5)` and `mul(11,8)` instructions are _disabled_ because there is a `don't()` instruction before them. The other `mul` instructions function normally, including the one at the end that gets re-_enabled_ by a `do()` instruction.

This time, the sum of the results is _`48`_ (`2*4 + 8*5`).

Handle the new instructions; _what do you get if you add up all of the results of just the enabled multiplications?_
