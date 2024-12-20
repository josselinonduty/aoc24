# Day 1: Historian Hysteria

[https://adventofcode.com/2024/day/1](https://adventofcode.com/2024/day/1)

## Description

### Part Two

Your analysis only confirmed what everyone feared: the two lists of location IDs are indeed very different.

Or are they?

The Historians can't agree on which group made the mistakes _or_ how to read most of the Chief's handwriting, but in the commotion you notice an interesting detail: <span title="We were THIS close to summoning the Alot of Location IDs!">a lot</span> of location IDs appear in both lists! Maybe the other numbers aren't location IDs at all but rather misinterpreted handwriting.

This time, you'll need to figure out exactly how often each number from the left list appears in the right list. Calculate a total _similarity score_ by adding up each number in the left list after multiplying it by the number of times that number appears in the right list.

Here are the same example lists again:

    3   4
    4   3
    2   5
    1   3
    3   9
    3   3

For these example lists, here is the process of finding the similarity score:

- The first number in the left list is `3`. It appears in the right list three times, so the similarity score increases by `3 * 3 = 9`.
- The second number in the left list is `4`. It appears in the right list once, so the similarity score increases by `4 * 1 = 4`.
- The third number in the left list is `2`. It does not appear in the right list, so the similarity score does not increase (`2 * 0 = 0`).
- The fourth number, `1`, also does not appear in the right list.
- The fifth number, `3`, appears in the right list three times; the similarity score increases by _`9`_.
- The last number, `3`, appears in the right list three times; the similarity score again increases by _`9`_.

So, for these example lists, the similarity score at the end of this process is _`31`_ (`9 + 4 + 0 + 0 + 9 + 9`).

Once again consider your left and right lists. _What is their similarity score?_
