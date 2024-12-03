# advent-of-claude

This year I'm declaring "Advent of Claude"!

Challenge: Write a Claude custom style to solve Advent of Code puzzles within Claude's UI.

Score: # adventofcode.com stars earned in 2 daily conversation turns.

Fine print: web app artifacts are allowed, including paste of your custom input into the artifact UI; one click only.

Per https://adventofcode.com/2024/about, wait until the daily http://adventofcode.com leaderboard is full before submitting LLM-generated solutions!

Of course, feel free to use ChatGPT custom instructions, static prompts, etc.

# My Progress 

* Day 1: ⭐⭐ https://claude.site/artifacts/d16e6bdb-f697-45fe-930c-7f58b2b5bb16
  * After solve, tweaked style to request an empty textarea in the artifact UI (prevent prefilled sample data which then needs to be deleted)
* Day 2: ⭐⭐ https://claude.site/artifacts/468f7f7f-c317-4c64-ab50-18943528e3c9
  * After solve, tweaked style to promote `lodash` use, explicit test cases, and separation of logic from UI; trimmed repetitive language.
* Day 3: ⭐⭐ https://claude.site/artifacts/3fee33db-a708-4839-89c0-2959481ac36f
  * After solve, some follow-up style explorations showe Claude getting very confused on `do_not_mul(5,5)` examples -- the curse of a just-smart-enough AI taking instructions too literally, or out of context! Maybe got lucky on this one, and curious if future puzzles will include any explicit anti-LLM flack. (I assume not, since the point of AoC is learning + self-directed fun... but it sure seems like the leaderboards are losing their meaning. Looking forward, maybe we'll see a bigger culture of screen-captured speedruns.) 
