## Johann Noronha

Aerospace engineer working in applied AI. I build systems that reason over messy real-world data — documents, video engagement, market signals — and I care most about the part everyone skips: knowing when the model is wrong. I like problems where the hard part isn't getting an answer, but trusting it.

Most of what I publish here is built end to end, from data pipeline to
interface, and tested against real inputs rather than curated demos.

www.linkedin.com/in/johann-noronha-345182271

---

### What I'm working on

**[Professor DAN](https://github.com/Jocodes23/Professor-DAN)** — a voice bot
for your own documents. Ask a question out loud and it answers out loud from
your PDFs, with the page or figure it used shown on screen, all running locally.
I built it because PaperMind got answers right but was too slow to talk to:
a verified answer took ~28 s and you could only type. Prof DAN starts speaking
about 3 s after you stop talking, on a laptop with a 4 GB GPU.

- **Two ways to talk.** *Voice chat* gives a short, precise answer as fast as
  possible. *Converse* is a hands-free conversation: it waits until you've
  finished your thought, replies to "thanks" or "go on" without searching the
  paper, and answers yes/no questions with a yes or no first.
- **Speaks while it thinks.** Speech is recognised while you're still talking,
  and the answer is streamed into speech sentence by sentence instead of
  waiting for it to finish.
- **Interrupt it any time.** Start talking and it stops mid-sentence.
- **Sources on screen before the first word.** Every answer shows the exact
  pages it came from.
- **Hears your project's words.** Speech recognition is biased toward
  vocabulary from your own documents, which cut a misheard key term from 39/54
  to 8/54 noisy test sentences.

`Python` · `FastAPI` · `faster-whisper` · `Silero VAD` · `Ollama (Qwen2.5)` · `Piper TTS` · `Chroma` · `Flutter`

**[PaperMind](https://github.com/Jocodes23/PaperMind)** — a local-first
document intelligence system for research papers. Answers are generated only
from the indexed corpus, every claim is entailment-checked against its source
by an NLI cross-encoder before it is returned, and any cited equation, figure
or table is displayed as the original page image so nothing has to be taken on
trust. Replacing LLM-based verification with a purpose-trained classifier cut
verification from ~60s to ~1s and eliminated a class of false rejections.

`Python` · `FastAPI` · `SQLite (sqlite-vec + FTS5)` · `Flutter` · `PyMuPDF` · `Transformers`

**[Reel Virality Analyser](https://github.com/Jocodes23/Reel-virality-analyser)**
— a trend-forecasting engine for short-form video that refuses to overclaim.
Hawkes/SEISMIC reproduction numbers, survival analysis and burst detection,
fused into calibrated probabilities with confidence intervals, validated by
temporal backtest against Brier score and expected calibration error. Adaptive
re-sampling reduced polling volume by ~75–79% versus fixed-interval collection,
and the whole pipeline runs real CLIP and MiniLM embeddings inside 4 GB of VRAM.

`Python` · `PyTorch` · `CLIP` · `scikit-learn` · `Docker`

**[Ai-TraderBot](https://github.com/Jocodes23/Ai-TraderBot)** — an event-driven
backtesting and strategy platform for Indian equities. Hand-rolled indicators,
meta-labelling with triple-barrier targets and purged cross-validation, and a
cost model reflecting real brokerage, STT and slippage. Results are reported as
measured rather than as marketing: most rule strategies are negative after
costs, and the chart-CNN experiment returned an out-of-sample AUC of 0.5001 —
recorded as the null result it is.

`Python` · `FastAPI` · `LightGBM` · `PyTorch` · `Flutter`

**[Style-Match Studio](https://github.com/Jocodes23/Style-Match-Studio)**
— reference-guided image generation that reproduces the visual language of an
inspiration post using your own content, then publishes it directly.

`TypeScript` · `Diffusion models`

**[Mail-to-drive](https://github.com/Jocodes23/Mail-to-drive)**
— scans a mailbox for matching messages and moves their attachments into Drive
entirely through browser automation, deliberately avoiding API and OAuth setup.

`Python` · `Browser automation`

---

### Background

B.Tech Aerospace Engineering, Amity University Mumbai (2021–2025), minor in Business Management. The move into AI wasn't a departure — it came from the same instinct that drove my engineering work: the hard part is understanding the problem clearly and being honest about what you don't know, not getting a machine to spit out an answer. I have work experience at a RAG company, and I've also worked on drones and other Aerospace vehicles.

---

### Interests

Voice interfaces and low-latency speech · retrieval systems and grounding ·
calibration and uncertainty · running capable
models on constrained hardware · anything where the interesting question is
"how do we know this is right?"

📫 johann.m.noronha@gmail.com
