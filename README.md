<h1 align="center">Johnny Kong</h1>

<p align="center">
  CS + Math student at the University of Michigan<br>
  <b>Low-latency C++. Real-time systems. LLM evals.</b>
</p>

<p align="center">
  <a href="mailto:johnnyxkong@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/kong-johnny"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
</p>

---

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

## 🛠️ Skills

**Languages**<br>
<img src="https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white" />
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" />
<img src="https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white" />
<img src="https://img.shields.io/badge/SQL-4479A1?style=flat-square" />
<br><br>

**Frameworks & Libraries**<br>
<img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=white" />
<img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" />
<img src="https://img.shields.io/badge/Angular-DD0031?style=flat-square&logo=angular&logoColor=white" />
<img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white" />
<img src="https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white" />
<img src="https://img.shields.io/badge/GoogleTest-4285F4?style=flat-square" />
<img src="https://img.shields.io/badge/Dear%20ImGui-2D2D2D?style=flat-square" />
<img src="https://img.shields.io/badge/ImPlot-2D2D2D?style=flat-square" />
<img src="https://img.shields.io/badge/Photon-34C759?style=flat-square" />
<br><br>

**Tools & Infrastructure**<br>
<img src="https://img.shields.io/badge/AWS%20Lambda-FF9900?style=flat-square&logo=amazonaws&logoColor=white" />
<img src="https://img.shields.io/badge/API%20Gateway-FF9900?style=flat-square&logo=amazonaws&logoColor=white" />
<img src="https://img.shields.io/badge/DynamoDB-4053D6?style=flat-square&logo=amazondynamodb&logoColor=white" />
<img src="https://img.shields.io/badge/Cognito-FF9900?style=flat-square&logo=amazonaws&logoColor=white" />
<img src="https://img.shields.io/badge/CloudWatch-FF4F8B?style=flat-square&logo=amazoncloudwatch&logoColor=white" />
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
<img src="https://img.shields.io/badge/SpacetimeDB-6E40C9?style=flat-square" />
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" />
<img src="https://img.shields.io/badge/Supabase-3FCF8E?style=flat-square&logo=supabase&logoColor=white" />
<img src="https://img.shields.io/badge/Stripe-635BFF?style=flat-square&logo=stripe&logoColor=white" />
<img src="https://img.shields.io/badge/Gemini%20API-4285F4?style=flat-square&logo=googlegemini&logoColor=white" />
<img src="https://img.shields.io/badge/GitLab-FC6D26?style=flat-square&logo=gitlab&logoColor=white" />
<img src="https://img.shields.io/badge/Ollama-000000?style=flat-square&logo=ollama&logoColor=white" />
<img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" />
<img src="https://img.shields.io/badge/CMake-064F8C?style=flat-square&logo=cmake&logoColor=white" />
<img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" />
<br><br>
