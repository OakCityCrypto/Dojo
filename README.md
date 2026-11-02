# Inequality Dojo

A belt-ranked math practice game for 7th grade. Students solve one move at a time and earn belts from White to Black (inequalities) and Yellow to Green (rotations).

**Play:** https://oakcitycrypto.github.io/Dojo/

[![Test](https://github.com/OakCityCrypto/Dojo/actions/workflows/test.yml/badge.svg)](https://github.com/OakCityCrypto/Dojo/actions/workflows/test.yml)

## What it teaches
| Track | Belts | Skill |
| --- | --- | --- |
| Inequalities | White, Blue, Purple, Brown, Black | Pick the box (A–D) → plus/minus → times/divide → flip? → graph |
| Rotations | Yellow, Orange, Green | Name the turn (watch 270°) → swap → change signs → plot |

Each belt test is 5 problems; 4 clean earns the belt. Progress saves in the browser on that device.

## Project layout
| Path | What |
| --- | --- |
| `index.html` | The whole game: one file, no build step |
| `tests/ci.js` | Release test suite: every belt, layout on 3 screens, accessibility, simulated students |
| `.github/workflows/test.yml` | Runs the suite on every change and every Monday |
| `docs/AGILE.md` | How sprints, the board, and releases work |
| `docs/TE-REPORT.md` | Latest test and evaluation results |
| `CHANGELOG.md` | What changed in each version |

## Run the tests yourself
```
cd tests
npm install
npx playwright install chromium
npm test
```
Screenshots and a full report land in `tests/out/`.
