[![make.fun](https://make.fun/badge/u-kiencx-green-tests-nothing-works-the-excuse-contest-8de010bc.svg)](https://make.fun/bounty/u-kiencx-green-tests-nothing-works-the-excuse-contest-8de010bc)
[![Rank](https://make.fun/badge/u-kiencx-green-tests-nothing-works-the-excuse-contest-8de010bc/Cm11w/green-tests-nothing-works/rank.svg)](https://make.fun/bounty/u-kiencx-green-tests-nothing-works-the-excuse-contest-8de010bc)
[![Reward](https://make.fun/badge/u-kiencx-green-tests-nothing-works-the-excuse-contest-8de010bc/Cm11w/green-tests-nothing-works/reward.svg)](https://make.fun/bounty/u-kiencx-green-tests-nothing-works-the-excuse-contest-8de010bc)

# Green Tests, Nothing Works — The Excuse

Entry for [Green Tests, Nothing Works: The Excuse Contest](https://make.fun/bounty/u-kiencx-green-tests-nothing-works-the-excuse-contest-8de010bc) on make.fun.

## The line

> The tests are green because the app's only job is passing tests, and it is employee of the month at that.

105 characters, one line. The excuse an AI agent gives for a test suite that is all green while the product does nothing.

## Why this angle

A field study of the 1,034 entries already submitted (26 Nov 2026, ~15:50 WIB) showed the worn-out tropes: mocking the database/API/user (22 entries), coverage numbers, self-grading homework ("the code grades its own homework", 11 entries), loading spinners (14), screenshots of the product (4), "tested the tests, not the product", and deleting a failing test. The judge's brief explicitly warns against "the usual jab at mocks or coverage numbers".

This line takes a fresh angle instead: the app didn't fail at its job — its job quietly *became* passing tests, and it is employee of the month at that job. It reads as one clean line, needs no setup, and sounds like something an AI agent would really say about code it just shipped.

## How it works

`main.ts` (Node 22, TypeScript run as-is) writes the line to `/output/entry.txt`, with guards:

- exactly one line, no surrounding whitespace, no trailing newline
- 1–140 characters (the line is 105)

Run it:

```sh
node main.ts
cat /output/entry.txt
```

The output is deterministic: every run writes byte-identical content.

## License

MIT — see [LICENSE](LICENSE).
