<h1 align="center">Johnny Kong</h1>

<p align="center">
  <b>Low-latency C++. Real-time systems. LLM evals.</b>
</p>

<p align="center">
  <a href="mailto:johnnyxkong@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/kong-johnny"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
</p>

---

## ⚔️ How I work

Profile it. Fix one thing. Measure again.

## 📌 Featured projects

### [⚡ orderbook](https://github.com/jkong07/orderbook) · C++20 / Python
A limit order book and market data feed handler. I prototyped it in Python, ported it to C++20 and tuned it one step at a time, benchmarking after every change.

- **~21.4–22.0M msgs/sec**, up from 660–710k in the naive baseline.
- **Overall p50 latency fell from 125ns to 41ns.**
- Optimizations in order: O(1) cancel through a hash-map index, array-indexed price levels, intrusive linked lists, a memory pool, then cache-line alignment.
- Replayed a full day of real Nasdaq ITCH data (via LOBSTER) with **0 invariant violations across 400,391 messages.**
- Fuzzed with a seeded random event generator that checks every invariant after each event.

### [🔥 flare](https://github.com/ardenk-svg/flare) · TypeScript · built at MHacks 2026
An incident-coordination simulation. A caller texts for help over iMessage, a human dispatches, and everyone sees the same live state.

- Gemini extracts structured facts from fragmented texts. Each fact keeps the exact quote behind it, and unknown stays `null`.
- Corrections like "south, not north" update the live incident instead of opening a new one.
- A deterministic rule table recommends services and a human decides. The model never assigns a unit.
- SpacetimeDB is the single source of truth, with role-checked reducers and live subscriptions. No polling.

### [🧮 math-prompting-eval](https://github.com/jkong07/math-prompting-eval) · Python
An empirical study of whether chain-of-thought, few-shot and self-consistency prompting still help on current open-source LLMs. It runs locally through Ollama on the MATH benchmark.

- Stratified sampling across all 5 difficulty levels.
- Compares 4 prompting strategies plus 8-sample self-consistency with majority voting.
- Pairwise significance testing with McNemar's test, plus accuracy broken down by difficulty.
- Reproducible runs: seeded sampling and JSON Lines results.

## 🛠️ Arsenal

<p>
  <img src="https://img.shields.io/badge/C++20-00599C?style=for-the-badge&logo=cplusplus&logoColor=white" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" />
  <img src="https://img.shields.io/badge/CMake-064F8C?style=for-the-badge&logo=cmake&logoColor=white" />
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" />
</p>

## 📊 Stats

<p align="center">
  <img height="170" src="https://github-readme-stats.vercel.app/api?username=jkong07&show_icons=true&hide_border=true&theme=transparent" />
  <img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=jkong07&layout=compact&hide_border=true&theme=transparent" />
</p>
