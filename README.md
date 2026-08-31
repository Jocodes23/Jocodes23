## Johann Noronha

Aerospace engineer working in applied AI. I build systems that reason over
messy real-world data — documents, video engagement, market signals — and I
care most about the part everyone skips: knowing when the model is wrong.

Most of what I publish here is built end to end, from data pipeline to
interface, and tested against real inputs rather than curated demos.

---

### What I'm working on

**[PaperMind](https://github.com/Jocodes23/PaperMind)** — a local-first
document intelligence system for research papers. Answers are generated only
from the indexed corpus, every claim is entailment-checked against its source
by an NLI cross-encoder before it is returned, and any cited equation, figure
or table is displayed as the original page image so nothing has to be taken on
trust. Replacing LLM-based verification with a purpose-trained classifier cut
verification from ~60s to ~1s and eliminated a class of false rejections.

`Python` · `FastAPI` · `SQLite (sqlite-vec + FTS5)` · `Flutter` · `PyMuPDF` · `Transformers`

**[Reels Trend Intelligence](https://github.com/Jocodes23/An-Instagram-reel-post-virality-predictor)**
— a trend-forecasting engine for short-form video that refuses to overclaim.
Hawkes/SEISMIC reproduction numbers, survival analysis and burst detection,
fused into calibrated probabilities with confidence intervals, validated by
temporal backtest against Brier score and expected calibration error. Adaptive
re-sampling reduced polling volume by ~75–79% versus fixed-interval collection,
and the whole pipeline runs real CLIP and MiniLM embeddings inside 4 GB of VRAM.

`Python` · `PyTorch` · `CLIP` · `scikit-learn` · `Docker`

**[Style-Match Studio](https://github.com/Jocodes23/Style-Matched-Auto-Posting-App)**
— reference-guided image generation that reproduces the visual language of an
inspiration post using your own content, then publishes it directly.

`TypeScript` · `Diffusion models`

**[Gmail → Drive automation](https://github.com/Jocodes23/Automation-without-the-use-of-apis)**
— scans a mailbox for matching messages and moves their attachments into Drive
entirely through browser automation, deliberately avoiding API and OAuth setup.

`Python` · `Browser automation`

---

### Background

B.Tech Aerospace Engineering, Amity University Mumbai (2021–2025), minor in
Business Management. Research intern at DIAT (DRDO) on subsonic aerodynamics
and CFD; earlier internships in aircraft maintenance at Air India and avionics
telemetry at Star Technology.

The move into AI came from the same instinct as the CFD work — most of the
difficulty is in modelling the thing honestly, not in running the solver.

---

### Interests

Retrieval systems and grounding · calibration and uncertainty · running capable
models on constrained hardware · anything where the interesting question is
"how do we know this is right?"

📫 mychajlo2303@gmail.com
