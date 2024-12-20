# Day 2: Red-Nosed Reports

[https://adventofcode.com/2024/day/2](https://adventofcode.com/2024/day/2)

## Description

### Part Two

The engineers are surprised by the low number of safe reports until they realize they forgot to tell you about the <span title="I need to get one of these!">Problem Dampener</span>.

The Problem Dampener is a reactor-mounted module that lets the reactor safety systems _tolerate a single bad level_ in what would otherwise be a safe report. It's like the bad level never happened!

Now, the same rules apply as before, except if removing a single level from an unsafe report would make it safe, the report instead counts as safe.

More of the above example's reports are now safe:

- `7 6 4 2 1`: _Safe_ without removing any level.
- `1 2 7 8 9`: _Unsafe_ regardless of which level is removed.
- `9 7 6 2 1`: _Unsafe_ regardless of which level is removed.
- `1 3 2 4 5`: _Safe_ by removing the second level, `3`.
- `8 6 4 4 1`: _Safe_ by removing the third level, `4`.
- `1 3 6 7 9`: _Safe_ without removing any level.

Thanks to the Problem Dampener, _`4`_ reports are actually _safe_!

Update your analysis by handling situations where the Problem Dampener can remove a single level from unsafe reports. _How many reports are now safe?_
