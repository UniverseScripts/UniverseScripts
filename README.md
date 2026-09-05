<div align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Geist+Mono&weight=600&size=24&pause=1000&color=3B82F6&center=true&vCenter=true&width=800&lines=Full-Stack+%26+AI+Infrastructure+Engineer;Bachelor+of+Artificial+Intelligence+(UTS);Backend+AI+Engineer+%E2%80%94+Internship+%40+FlyRank+AI;Cheap+fast+paths+gating+expensive+slow+ones" alt="Typing SVG" />
</div>

<p align="center">
  <a href="https://yoshio-nomura.vercel.app"><img src="https://img.shields.io/badge/Portfolio-yoshio--nomura.vercel.app-3b82f6?style=flat-square&labelColor=18181b" alt="Portfolio"></a>
  <a href="https://github.com/UniverseScripts"><img src="https://img.shields.io/badge/Level-Undergraduate_%2F_Intern-09090b?style=flat-square&labelColor=18181b" alt="Level"></a>
  <a href="https://vercel.com"><img src="https://img.shields.io/badge/Deployment-Vercel-3b82f6?style=flat-square&labelColor=18181b" alt="Vercel"></a>
  <a href="https://galacticgamer62.gumroad.com"><img src="https://img.shields.io/badge/Products-Gumroad-10b981?style=flat-square&labelColor=18181b" alt="Gumroad"></a>
</p>

<div align="center">
  <img src="https://github-stats-extended.vercel.app/api/top-langs?username=UniverseScripts&layout=donut-vertical&langs_count=4&theme=tokyonight&hide_border=true&bg_color=09090b&title_color=3b82f6&text_color=fafafa" alt="Top Languages" width="48%"/>
</div>

### ── The thread running through all of it

A cheap decision placed in front of an expensive one.

An XGBoost classifier scores ICU stream events in under 5 ms and only then pays for an LLM call.
A local Qwen 2.5 3B model reads a task's difficulty and routes it before a cloud API is touched.
Same idea twice, and it is the part of this work I would defend in an interview.

### ── Stack

<div align="center">
  <img src="https://skillicons.dev/icons?i=python,ts,java,fastapi,pytorch,react,nextjs,tailwind,postgres,redis,docker,githubactions,git,vercel&theme=dark" alt="Tech Stack" />
</div>

### ── Projects

Every figure below is stated with the conditions it was measured under. Where a project has no
number, it is because nothing was instrumented — not because the number was disappointing.

<table>
  <tr>
    <td width="50%" valign="top">
      <strong>🩺 Pulsemind</strong><br/>
      <i>Critical-care telemetry — research prototype</i><br/><br/>
      An asynchronous ICU telemetry processor. An XGBoost classifier scores incoming stream events and gates higher-cost LLM rationalisation calls so they fire only on detected anomalies.<br/><br/>
      <code>Team — full-stack AI engineer</code><br/>
      <code>May 2026 — ongoing</code><br/>
      <code>Python · XGBoost · PyTorch · scikit-learn · React</code><br/><br/>
      Classifier forward pass <strong>&lt;5 ms</strong> per stream event.<br/>
      End-to-end <strong>&lt;50 ms</strong>; the anomaly path additionally incurs the ~15 s LLM step.<br/><br/>
      <sub>Trained on the credentialed MIMIC-IV (PhysioNet) de-identified ICU dataset under its DUA; demos run on a synthetic derivative. No clinical deployment.</sub>
    </td>
    <td width="50%" valign="top">
      <strong>🧠 Develarper</strong><br/>
      <i>LLM task routing</i><br/><br/>
      A two-tier router built solo for the AMD Developer Hackathon (Act II). A local Qwen 2.5 3B classifier scores task difficulty and dispatches hard tasks to Fireworks while easy ones stay local.<br/><br/>
      <code>Solo — LLMOps</code><br/>
      <code>July 2026 · AMD Developer Hackathon, Act II</code><br/>
      <code>Python · Qwen 2.5 3B via Ollama · FastAPI · Fireworks</code><br/><br/>
      Routing: <strong>18 of 19</strong> tasks to the correct tier, on self-defined labels.<br/>
      Answer quality: <strong>93.00%</strong> (186/200) over 100 factual + 100 summarization tasks, scored by similarity/Jaccard overlap against expected answers — not human or LLM review. Mean latency <strong>505.1 ms</strong>, sequential.<br/><br/>
      <sub>6 of the 200 prompts contain unrendered template placeholders and are unanswerable as posed. Raw results are committed in the repo.</sub>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <strong>⚡ Roomie</strong><br/>
      <i>Roommate and apartment matching</i><br/><br/>
      Onboarding survey and swipe interface matching on structured fields, with an optional free-text bio path using Vertex AI embeddings and cosine similarity.<br/><br/>
      <code>Contributor, team of 4 — DevOps & Backend Engineering</code><br/>
      <code>April 2026 · GDGoC National Hackathon 2026 (Hanoi), team Hackaphobia</code><br/>
      <code>Python · FastAPI · React · PostgreSQL · Vertex AI</code><br/><br/>
      <strong>~50</strong> real users onboarded and swiped at demo day.<br/>
      <strong>~12 ms</strong> average request latency — structured matching path only, excluding embedding generation.
    </td>
    <td width="50%" valign="top">
      <strong>🌩️ Weatherise</strong><br/>
      <i>Weather-intelligence pipeline</i><br/><br/>
      REST sources and NVIDIA Earth-2 surrogate models feeding a multi-agent chain on Nemotron Ultra, with a Qdrant vector database supporting RAG over the ingested data.<br/><br/>
      <code>Team — LLMOps & Backend AI Engineering</code><br/>
      <code>9–11 June 2026 · Vietnam AI Open Hackathon (NVIDIA / OpenACC)</code><br/>
      <code>Python · Qdrant · Earth-2 · Nemotron Ultra · MCP</code><br/><br/>
      <sub>Demonstrated at concurrency 1 over three days. No latency or throughput figure is stated, because none was measured under load.</sub>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <strong>🗺️ Vora</strong><br/>
      <i>Quiz-verified learning roadmap</i><br/><br/>
      A deployed learning-roadmap application with quiz-gated progression. The backend resolver converts unstructured model output into validated, dependency-mapped directed acyclic graphs.<br/><br/>
      <code>Team — backend engineer</code><br/>
      <code>April 2026 · GDGoC DevCamp, HCMUT</code><br/>
      <code>React Flow</code><br/><br/>
      <sub>Cycle detection is O(V+E) — an algorithmic property of the traversal, not a measured latency.</sub>
    </td>
    <td width="50%" valign="top">
      <strong>🧪 ArchitectureLab</strong><br/>
      <i>WebMCP architecture studio</i><br/><br/>
      A shared live system model where a person and an agent inspect the same request flow. The agent calls structured tools the page registers and cannot change anything without approval.<br/><br/>
      <code>Solo</code><br/>
      <code>August 2026 · OpenAI WebMCP Challenge</code><br/><br/>
      <sub>Every number in the simulator is synthetic and directional — stated assumptions, not measurements.</sub>
    </td>
  </tr>
</table>

### ── Credentials

| Credential | Issuer | Type | Issued |
| :--- | :--- | :--- | :--- |
| **Dean's List 2026** | University of Technology Sydney | Honour | 2026-07-09 |
| **Certificate of Attendance** | Vietnam AI Open Hackathon (NVIDIA / OpenACC) | Attendance | 2026-06-09 |
| **Top 30 Finalist Award** | GDGoC National Hackathon 2026 (Hanoi) | Placement | 2026-05-20 |
| **Next.js App Router Fundamentals** | Vercel | Completion | 2026-02-20 |
| **Generative AI with Large Language Models** | DeepLearning.AI & AWS — via Coursera | Completion | 2026-01-02 |
| **AWS Cloud Practitioner Essentials** | Amazon Web Services | Foundational completion | 2025-12-03 |

<sub>On the NVIDIA entry: the certificate is one of attendance. The claimable part is that the team was <strong>selected as one of 10 from roughly 100 registrants</strong> to compete. It was a one-round event and the team did not place.</sub>

### ── Products

* 📦 **[Local RAG API](https://galacticgamer62.gumroad.com/l/local-rag-api)** — a self-hosted retrieval-augmented generation API layer that runs on your own hardware.
* ⚡ **[Next.js Mobile Starter Kit](https://galacticgamer62.gumroad.com/l/nextjs-mobile-marketplace)** — a Next.js starter configured for mobile-first static export.
* 📊 **[Global Tech Intelligence Node](https://galacticgamer62.gumroad.com/l/job-weekly)** — a curated weekly feed of technology and infrastructure signals.

### ── Elsewhere

* [LinkedIn](https://www.linkedin.com/in/yoshio-nomura-b3219438b)
* [X](https://x.com/Asterios07)
* [YouTube](https://www.youtube.com/@AsteriosTech) · [TikTok](https://www.tiktok.com/@asteriostech) · [Instagram](https://www.instagram.com/asteriostech/)
