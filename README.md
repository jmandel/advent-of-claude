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
  * After solve, some follow-up style explorations showed Claude getting very confused on `do_not_mul(5,5)` examples -- the curse of a just-smart-enough AI taking instructions too literally, or out of context! Maybe we got lucky that today's first samples avoided this pitfall. I'm curious to see if future puzzles will include any explicit anti-LLM flak. (I assume not, since the point of AoC is learning + self-directed fun... but it sure seems like the leaderboards are losing integrity. Looking forward, maybe we'll see a bigger culture of screen-captured speedruns.)
* Day 4: ⭐⭐ (*) https://claude.site/artifacts/f5edfce1-fda7-443b-afce-fe74c7a1a36b
  * On Part 2, Claude took 4 code analyzer blocks to fully debug its algorithm. (It's rare in my experience that broken code gets fixed after three failed attempts, so this was a pretty impressive feat.) Then Claude hit a token output limit while finishing transcribing the solution into a web app. So I spent a third turn saying "Continue," and it emitted the final HTML tags. I'm counting this as a moral success, but it technically violates my pre-specified terms.
  * After solve, updated style to provide more debugging advice, more functional programming guidance, and an example that uses lodash
* Day 5: ⭐⭐ https://claude.site/artifacts/5fa3423f-5dbb-41a9-a52e-0bba8c6fcd68
  * No notes
* Day 6: Zero stars https://claude.site/artifacts/9ee7b9c7-a33e-403d-afa9-0cc5d9bb7a39
  * At several points, Claude created infinite loops in the JS REPL, saw the timeout error, and figured "Great, that code's fine let's proceed to make a web app now." I've mitigated this with a style update.
  * Moreover, Claude had a really hard time internalizing some of the constraints here. About half the time, it insisted on treating obstacles and grid boundaries the same (instead of treating obstacles as things that make you turn, and grid boundaries as termination conditions for the path). I wound up providing specific hints for Part 1 and Part 2
    * Example: "Careful that you don't treat grid-exiting like a boundary. And improve perf by only x,y positions on the default path as the potential insertion points for the new obstacle." 
* Day 7: ⭐⭐ https://claude.site/artifacts/6507ffb5-dc75-4a44-9837-ed7a3379471c
  * Solved in with no trouble (although I got distracted and accidentally submitted my Part 2 solution before the leaderboard was full -- d'oh)
  * Part 2 solution was annoyingly slow, so I followed up with "Try recursive algo where you bail if the interim value is too high" to get the app above
* Day 8: ⭐⭐ https://claude.site/artifacts/0259a9d6-e541-4949-ab71-5bad2da3aaf4
  * Algorithm is N²K² for NxN grid with K antennas in the biggest group. This could easily be reduced by a factor of N, but in practice it runs instantaneously on the supplied input
* Day 9: ⭐⭐ https://claude.site/artifacts/fbe5c368-98c5-46b4-a92a-e35742920575
* Day 10: ⭐⭐ https://claude.site/artifacts/f8d5d315-8cd3-4602-8854-f4ad77560151
* Day 11: ⭐ https://claude.site/artifacts/55e0f02f-4594-45e8-ae67-ecabeb8c41f9
  * Failed to pursue an efficient strategy for Part 2 -- one star only
  * Asked o1 to fix, for the solution above 
* Day 12: ⭐ https://claude.site/artifacts/20881e52-6a4e-4790-97ea-88c192b97ee8
  * Claude really struggled with the wall following. Even with a very explicit prompting about the algorithm, I had carefully debug and explain what was going wrong.
* Day 13: ⭐
* Day 14: ⭐
* Day 15: Zero stars
