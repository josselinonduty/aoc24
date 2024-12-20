# Day 7: Bridge Repair

[https://adventofcode.com/2024/day/7](https://adventofcode.com/2024/day/7)

## Description

### Part Two

The engineers seem concerned; the total calibration result you gave them is nowhere close to being within safety tolerances. Just then, you spot your mistake: some well-hidden elephants are holding a _third type of operator_.

The [concatenation](https://en.wikipedia.org/wiki/Concatenation) operator (<span title="I think you mean &quot;.&quot;.">`||`</span>) combines the digits from its left and right inputs into a single number. For example, `12 || 345` would become `12345`. All operators are still evaluated left-to-right.

Now, apart from the three equations that could be made true using only addition and multiplication, the above example has three more equations that can be made true by inserting operators:

- `156: 15 6` can be made true through a single concatenation: `15 || 6 = 156`.
- `7290: 6 8 6 15` can be made true using `6 * 8 || 6 * 15`.
- `192: 17 8 14` can be made true using `17 || 8 + 14`.

Adding up all six test values (the three that could be made before using only `+` and `*` plus the new three that can now be made by also using `||`) produces the new _total calibration result_ of _`11387`_.

Using your new knowledge of elephant hiding spots, determine which equations could possibly be true. _What is their total calibration result?_
