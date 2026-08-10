## Hi, I'm Shaif 👋

**RF & Satellite Communications Engineer** · UK 🇬🇧 · MSc Mobile & Satellite Communication (Distinction)

### 🚀 Featured Project

**[🛰️ Overpass — live 5G-NTN pass analyzer](https://overpass.streamlit.app)**
Pick any of 40+ cities worldwide and see what a 5G phone would experience from a satellite passing overhead — link quality, data rate, sync cost, handover and latency — from real orbital data, self-refreshed daily.

▶️ **Try it live: [overpass.streamlit.app](https://overpass.streamlit.app)** · 💻 [Source & 12-week portfolio](https://github.com/shaifiqbal/ntn-flagship)

---

Building open engineering tools at the intersection of **AI · 5G/6G · Satellite (Non-Terrestrial Networks)**.

I design and integrate RF and SDR systems — I built the University of South Wales' first operational satellite ground station end-to-end, and I've delivered large-scale 4G/5G RAN programmes across multiple operators. Right now I'm building a public series of small, real, tested tools exploring how AI meets satellite communications.

`MIET` · `IEEE` · `IEEE ComSoc` · `SSPI` · Finalist, Airbus Space Competition UK 2024

---

### 🛰️ 12-Week NTN Engineering Series

A build-in-public series analysing **5G Non-Terrestrial Networks** — the technology connecting phones directly to low-orbit satellites like Starlink — using **real, live satellite data** rather than textbook assumptions.

One engineering problem per week, each with working code, a passing test suite, and an honest write-up — **including the results where the simple approach beat the clever one.** The weeks build from "can we see a satellite" through sync, handover, throughput and latency, into a single tool that runs the whole chain end to end.

**👉 Start here — [ntn-toolkit](https://github.com/shaifiqbal/ntn-toolkit):** the whole series tied together. One command produces a full pass report — geometry, link, throughput, pre-compensation, handover and latency — from live satellite data.

**Can we see it? (visibility & orbits)**
- **[ntn-link-budget](https://github.com/shaifiqbal/ntn-link-budget)** — Satellite link budget calculator: does the link close, across elevation angles? (FSPL → C/N0 → Eb/N0 → margin)
- **[ntn-pass-predictor](https://github.com/shaifiqbal/ntn-pass-predictor)** — Feeds a *real* live Starlink pass (Celestrak + SGP4) into the link budget — real elevation, range and Doppler over an actual pass over Aberdeen
- **[ntn-multi-sat-scheduler](https://github.com/shaifiqbal/ntn-multi-sat-scheduler)** — Tracks several live satellites at once and decides which one should carry the link, detecting real hand-off events
- **[ntn-sat-predictor-ml](https://github.com/shaifiqbal/ntn-sat-predictor-ml)** — Machine-learning model for satellite visibility duration, with an honest comparison of greedy vs ML hand-off (Random Forest + SGP4)

**Can we stay in sync? (5G timing, Doppler & pre-compensation)**
- **[ntn-5g-timing-doppler](https://github.com/shaifiqbal/ntn-5g-timing-doppler)** — Where standard 5G NR breaks over a satellite: timing advance and Doppler measured against real 3GPP limits
- **[ntn-5g-ntn-precomp](https://github.com/shaifiqbal/ntn-5g-ntn-precomp)** — 3GPP Release-17 GNSS-assisted pre-compensation over a real pass, and how often it must be refreshed
- **[ntn-adaptive-precomp](https://github.com/shaifiqbal/ntn-adaptive-precomp)** — Adaptive vs fixed refresh scheduling — an honest result: timing binds, and a well-chosen fixed rate is hard to beat

**Which satellite, and how much data? (handover, throughput, latency)**
- **[ntn-precomp-aware-handover](https://github.com/shaifiqbal/ntn-precomp-aware-handover)** — Strongest-signal vs cheapest-to-sync handover — they turn out to mostly agree, and here's why
- **[ntn-link-adaptation](https://github.com/shaifiqbal/ntn-link-adaptation)** — SNR → CQI → throughput over a pass: visibility isn't capacity — most data arrives in a short high-elevation window
- **[ntn-latency-budget](https://github.com/shaifiqbal/ntn-latency-budget)** — Propagation delay, HARQ and TCP over a pass: HARQ stalling is numerology-dependent

**Bringing it together**
- **[ntn-toolkit](https://github.com/shaifiqbal/ntn-toolkit)** — One package running the whole chain end to end into a single live pass report + dashboard
- **[ntn-flagship (Overpass)](https://github.com/shaifiqbal/ntn-flagship)** — the capstone: a live web app wrapping the whole toolkit. Pick any of 40+ cities and see the full 5G-NTN pass analysis in your browser. ▶️ **[Try it live](https://overpass.streamlit.app)**

---

### 🔧 Tools I use

- **Python** — the whole portfolio
- **Skyfield + SGP4** — propagating satellite orbits from real data
- **Live TLE data from Celestrak** — the actual current positions of Starlink satellites
- **scikit-learn** — the machine-learning parts
- **NumPy · Matplotlib · pandas** — computation and plots
- **pytest** — every project has a passing test suite
- **3GPP standards** — 5G parameters (timing budgets, frequency tolerances, HARQ, CQI tables) grounded in the actual telecom specs, not made-up numbers
- **Git / GitHub** — everything public and MIT-licensed, so anyone can use it

Also: `MATLAB` · `SDR (SDRplay, ICOM)` · `Ansys STK` · `RF & antenna integration` · `3GPP (RAN1/RAN4)` · `OSS/EMS`

---

### 📜 Certifications

![Microsoft](https://img.shields.io/badge/Microsoft%20Certified-Azure-0078D4?style=flat&logo=microsoftazure&logoColor=white) ![Python](https://img.shields.io/badge/Python%203-University%20of%20Michigan-3776AB?style=flat&logo=python&logoColor=white)

**Microsoft Azure**
- Microsoft Certified: [Azure Solutions Architect Expert](https://learn.microsoft.com/en-us/users/shaif-8163/credentials/c2a8078643789f57)
- Microsoft Certified: Azure AI Engineer Associate
- Microsoft Certified: Azure Security Engineer Associate
- Microsoft Certified: Azure Administrator Associate
- Microsoft Certified: Azure Virtual Desktop Specialty

**Programming**
- [Python 3 Programming Specialization](https://www.coursera.org/account/accomplishments/specialization/VVHXJHBF6JCC) — University of Michigan (Coursera)

---

### ✍️ I write about this too

- **Medium:** [@shaifiqbal](https://medium.com/@shaifiqbal) — technical write-ups on each project
- **Newsletter:** [The Signals AI](https://www.thesignalsai.com) — build-in-public, plain-language version of each week
