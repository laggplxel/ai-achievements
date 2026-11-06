# AI Achievements

Everything here is generative AI: LLMs and other transformers, diffusion models, and GANs. Same family of tech as chatbots and "AI art."

---

## Start here

If you only open six links, open these. Each one has someone outside the AI company vouching for it.

1. **The KLS conjecture (open since 1995) is proved, and the experts credit ChatGPT.** Bizeul, Klartag and Lehec, the people who made the previous big progress on this exact problem, say in their own paper that most of the proofs and ideas in it were found by ChatGPT. [Paper](https://arxiv.org/abs/2610.05474)

2. **An 80-year-old Erdős conjecture disproved, and Fields Medalist Tim Gowers says he'd have accepted it into the Annals of Mathematics.** An OpenAI model disproved the unit distance conjecture in one shot. Nine outside mathematicians checked it, and Gowers wrote he "would have recommended acceptance without any hesitation." [OpenAI](https://openai.com/index/model-disproves-discrete-geometry-conjecture/) · [Mathematicians' paper](https://arxiv.org/abs/2605.20695)

3. **The Jacobian conjecture (open since 1939) is false, and you can check it with a calculator.** Mathematician Levent Alpöge and Claude found a counterexample short enough to fit in a tweet. Terence Tao checked it, and it's been formally verified in Isabelle. [Wikipedia](https://en.wikipedia.org/wiki/Jacobian_conjecture#Counterexample_for_n_%3E_2) · [Formal verification](https://isa-afp.org/entries/Jacobian_Counterexample.html)

4. **Claude broke a physics record, and the record holder verified it himself.** Claude computed a scattering amplitude at nine loops, one past the eight-loop record SLAC's Lance Dixon set in 2023. Dixon checked it. [Anthropic](https://www.anthropic.com/research/yes-claude-can-do-nine-loops)

5. **Google's AI-built flu forecaster beat the CDC's own forecast.** It ranked #1 of 39 models in the CDC's 2025–26 season evaluation. The CDC's official ensemble came 7th. The forecasts were made before the outcomes were known, and the CDC did the scoring. [Google](https://blog.google/innovation-and-ai/models-and-research/google-research/google-science-ai-flu-forecasts/)

6. **The Erdős–Szemerédi sunflower conjecture (from 1978) is proved, and the mathematicians credit ChatGPT with the key argument.** [Paper](https://arxiv.org/abs/2610.26686)

---

## Mathematics

**A Millennium Prize problem: Navier–Stokes.** About 10,000 OpenAI agents worked for 88 hours and produced a proof that the 3D Navier–Stokes equations can blow up in finite time, formalized in Lean. Quanta Magazine's headline: "AI Has Solved One of Math's $1 Million Millennium Prize Problems." [OpenAI](https://openai.com/index/navier-stokes-solution/)

**The Kakeya conjecture in every dimension.** Humans only proved the 3D case in 2025 (Hong Wang and Joshua Zahl). OpenAI's model proved Sogge's local smoothing conjecture (from 1991) in every dimension, which gives Kakeya in every dimension at once. Formalized in Lean. [Paper](https://github.com/openai/math/blob/main/preprints/Local-smoothing-for-the-Euclidean-wave-equation-October-25-2026/paper.pdf)
Before that, it had already done Kakeya in [4 dimensions](https://github.com/openai/math/blob/main/preprints/Every-four-dimensional-Kakeya-set-has-full-Hausdorff-dimension-September-24-2026/paper.pdf) and the stronger "maximal" version in [3 dimensions](https://github.com/openai/math/blob/main/preprints/The-Kakeya-maximal-conjecture-in-three-dimensions-September-23-2026/paper.pdf).

**The quasi-Riemann hypothesis.** The Riemann zeta function has no zeros with real part above 7/8. Formalized in Lean, so anyone can machine-check it. [Paper](https://github.com/openai/math/blob/main/preprints/The-Quasi-Riemann-Hypothesis-September-30-2026/paper.pdf)

**Over two thirds of the Riemann zeta zeros are on the critical line.** The best proven fraction had been 41.6%. Claude pushed it to 67.2%. Number theorists Brian Conrey and Dan Goldston reviewed it, and it's formalized in Lean. [Anthropic](https://www.anthropic.com/research/riemann-zeta) · [Paper](https://arxiv.org/abs/2608.13637)

**Hilbert's tenth problem over the rationals.** No algorithm can decide whether a polynomial equation has a rational solution. [Paper](https://github.com/openai/math/blob/main/preprints/Hilberts-tenth-problem-over-the-rational-numbers-September-24-2026/main.pdf)

**The Hopf problem (from 1947): does the 6-sphere have a complex structure?** Levent Alpöge, working with Claude, posted a 108-page proof that the answer is yes. Scientific American covered it, and other mathematicians are already writing papers that build on it. [Paper](https://alpo.ge/s6.pdf) · [Scientific American](https://scientificamerican.com/article/ai-solves-79-year-old-math-mystery-of-six-dimensional-spheres)
It also overturns a peer-reviewed result. In 2020, Campana, Demailly and Peternell published in Compositio Mathematica (Corollary 2.3) that any complex structure on the 6-sphere must have algebraic dimension 0. The new construction has algebraic dimension 1. The paper says outright that "the two statements cannot both be correct," and it has a section titled "Why the argument of [CDP20] does not apply" that pinpoints the step where the published argument breaks down. If it were just literature searching, it would have taken that publication as gospel, because that's how academia treats peer review. It didn't. [The 2020 paper](https://www.cambridge.org/core/journals/compositio-mathematica/article/algebraic-dimension-of-compact-complex-threefolds-with-vanishing-second-betti-number/CDF2D04CFB35CEE105E10B188D97D68A)

**The Erdős–Hajnal conjecture for every path.** One team says their proof was developed through an interactive dialogue with Claude Opus 5.5 and ChatGPT-6. It went public on October 7, ten days before the leading human expert on the problem posted his own independent proof. [AI-assisted proof](https://arxiv.org/abs/2611.01963) · [Independent proof](https://arxiv.org/abs/2610.24887)

**The cycle double cover conjecture (about 50 years old).** OpenAI's paper says the proof is "entirely due to GPT 5.6 Sol Ultra." Graph theorists have since written their own expositions of it. [OpenAI proof](https://cdn.openai.com/pdf/04d1d1e4-bc75-476a-97cf-49055cd98d31/cdc_proof.pdf) · [Exposition](https://arxiv.org/abs/2607.16356) · [Another exposition](https://arxiv.org/abs/2607.15399) · [Post](https://x.com/__eknight__/status/2075643450196971805)

**The unit distance conjecture, again, this time peer-reviewed.** A researcher used a public model, GPT-5.5 Pro, to independently produce disproofs, published in PNAS. So this isn't some secret internal model. [PNAS](https://www.pnas.org/doi/abs/10.1073/pnas.2621541123)

**The Dinitz–Garg–Goemans conjecture (about 30 years old).** GPT-5.6 Pro broke it with four prompts totaling under 60 words. The counterexample is small enough that anyone can check it. [Post](https://x.com/DmitryRybin1/status/2079904005652893709)

**A decades-old statistics question about the Benjamini–Hochberg procedure.** Penn statistician Edgar Dobriban asked GPT-5.6 Pro to prove or disprove it. About 90 minutes later it returned a proof, a counterexample, and code to verify both. Dobriban checked all of it himself. [Post](https://x.com/EdgarDobriban/status/2077082912021786660)

**Erdős problem #1196.** A 23-year-old with no advanced math degree gave GPT-5.4 Pro the problem statement, and it solved it. [Chat log](https://chatgpt.com/share/69dd1c83-b164-8385-bf2e-8533e9baba9c) · [Problem page](https://www.erdosproblems.com/1196)
Mathematicians including Terence Tao, widely considered the greatest living mathematician, have looked at it, and a paper on it describes a new method "suggested from output of GPT-5.4 Pro." Keyword: new. [Paper](https://arxiv.org/abs/2605.00301)

**Ten decade-old problems in one release, all Lean-checked.** These include Erdős problems 146, 180 and 183, and the first improvement to the general sphere-packing exponent since 1978. By OpenAI's estimate, all ten together cost about $2,000 in compute. [Paper](https://cdn.openai.com/pdf/ten-proofs-oai.pdf)

**Longer gaps between primes.** A new bound on the largest gap between consecutive primes. The paper says the proof is due to GPT 6 Astra, and there's a complete Lean proof. [Paper](https://cdn.openai.com/pdf/51126fac-1b68-4128-9666-c908bcc16033/long_gaps.pdf)

**DeepMind's AlphaProof Nexus, peer-reviewed in Science.** It autonomously solved 9 open Erdős problems (two of them open since 1970) and 44 open conjectures from the OEIS integer-sequence database, each with a machine-checkable proof. [Paper](https://arxiv.org/abs/2605.22763)

**Fermat's Last Theorem, fully formalized in 11 days.** Claude wrote 13 million lines of Lean, the first complete computer-checked proof of the theorem. It's a formalization of Wiles's proof rather than a new one, and the community had expected it to take years. Kevin Buzzard, who leads the human effort, reviewed it. [Anthropic](https://www.anthropic.com/research/formalizing-fermats-last-theorem)

**The whole OpenAI math dump: 721 manuscripts across 373 result families.** [Repository](https://github.com/openai/math) · [Overview](https://github.com/openai/math/blob/main/overview.pdf)
A summary of the biggest ones counts 90 of the 500 most important open problems in math as solved. [Thread](https://x.com/aisafetymemes/status/2107622121618964829)

More: [vibemathed.com](https://vibemathed.com/)

---

## Theoretical computer science

**The Exponential Time Hypothesis is false.** Since 1999, ETH said 3-SAT can't be solved meaningfully faster than exponential time, and Claude's literature search found over 800 papers built on it or on something stronger. On October 16, 2026, an OpenAI model and a Claude model each independently found a subexponential algorithm, on the same day. Both are formalized in Lean, and the people who proposed ETH are running the review themselves. [OpenAI paper](https://github.com/openai/math/blob/main/preprints/The-Exponential-Time-Hypothesis-is-False-October-25-2026/paper.pdf) · [Anthropic paper + Lean proof](https://github.com/anthropics/formal-math/tree/main/eth)

**Truly subquadratic 3SUM and truly subcubic APSP.** The 3SUM and APSP hypotheses are two of the central "you can't go faster than this" assumptions of fine-grained complexity, and this paper by Josh Alman and Virginia Vassilevska Williams beats both. The paper says an Anthropic employee used an internal research model to investigate open problems in the theory of cryptography, and Anthropic released a Lean formalization of the results. It looks incremental, but it's like finding out you can go 1.000004x the speed of light: tiny on paper, but the wall was supposed to be unbreakable. [Paper](https://arxiv.org/html/2610.06783v1#Sx1.SS0.SSS0.Px1) · [Lean formalization](https://github.com/anthropics/formal-math/tree/main/3sum-apsp)

**The Aaronson–Ambainis conjecture (open since 2008) is proved, and the proof is checked in Lean.** It's one of the central open problems in quantum computing: it says exponential quantum speedups need structure, and that on almost all inputs a classical algorithm can approximate a quantum one with only polynomially more queries. In 2019, two mathematicians announced a proof, and it turned out to have a subtle flaw. Physical Superintelligence's research system, running instances of an unreleased Anthropic model, wrote down a complete proof on the third day of its run, then pushed the bound's exponent from 22 down to 7. Lean's kernel checked it with no unproven assumptions, and Scott Aaronson himself pointed PSI to a team of complexity theorists who are writing up an exposition of the proof for experts. [Paper](https://github.com/physical-superintelligence/aaronson-ambainis/blob/main/paper/aaronson_ambainis_paper.pdf) · [Lean proof](https://github.com/physical-superintelligence/aaronson-ambainis) · [The flawed 2019 attempt](https://arxiv.org/html/2402.13952v2)

---

## Physics

**Yang–Mills existence, half of a Millennium Prize problem.** OpenAI's model produced a rigorous existence proof for pure Yang–Mills theory in 4 dimensions, then for QCD, the theory of quarks and gluons. Physicists have used these theories for decades without a proof that they mathematically exist. Nobel laureate David Gross is reviewing it. The mass gap half is still open. [Background](https://en.wikipedia.org/wiki/Yang%E2%80%93Mills_existence_and_mass_gap)

**49 of 50 unpublished research-level physics problems.** Physicists wrote 50 brand-new problems that take an expert a day or more each. GPT-6 Astra got 49 right at under $3 per problem. At first it scored lower, because in several cases it insisted the experts' answer keys were wrong. It was right. [Paper](https://arxiv.org/abs/2610.16733)

**Nine loops:** see Start here. [Anthropic](https://www.anthropic.com/research/yes-claude-can-do-nine-loops)

---

## Medicine, chemistry and biology

### LLMs

**AI beat doctors at diagnosis in Science.** On real emergency-room cases at the first decision point, OpenAI's o1 got the correct or near-correct diagnosis about 67% of the time, versus 50–55% for expert physicians. [Paper](https://www.science.org/doi/10.1126/science.adz4433)

**18 new rare-disease diagnoses that years of specialists couldn't crack.** Doctors used OpenAI's o3 on 376 previously unsolved rare-disease cases. The model surfaced the leads, and every diagnosis was confirmed clinically. [OpenAI](https://openai.com/index/diagnose-rare-childhood-diseases/) · [NEJM AI paper](https://ai.nejm.org/doi/full/10.1056/AIcs2501343?query=featured_home)

**Claude found a new CRISPR-like enzyme system.** About 950 Claude agents searched more than 200,000 enzymes in 21 hours and spotted a system nobody had recognized. CRISPR pioneer Feng Zhang called the connection "genuinely intriguing." Nobody knows yet what it does. [Anthropic](https://www.anthropic.com/news/claude-discovers-novel-enzyme-system)

**Claude designs proteins as well as top human experts.** It designed binders against 14 of 15 targets, with hit rates over 20% versus the typical 10–15%. Independent labs built and tested the designs. [Anthropic](https://www.anthropic.com/research/Claude-accelerates-protein-design)

**Claude designed proteins against scorpion toxins.** It worked mostly on its own for 64 hours. Independent labs tested 211 designs, and 17 bound their targets. [Anthropic](https://www.anthropic.com/research/claude-scorpion-toxin-binder-design)

**GPT-5 made a lab technique 79x more efficient.** It improved a standard molecular cloning protocol over several rounds of real lab experiments, introducing a mechanism of its own. [OpenAI](https://openai.com/index/accelerating-biological-research-in-the-wet-lab/)

**A lab run by LLM agents, published in Nature.** AutoDNA's agents coordinate 20+ kinds of lab instruments and have run more than 11,000 experimental steps, matching results that human experts published. [Nature](https://www.nature.com/articles/s41586-026-11228-6)

**A team of AI scientists designed new COVID nanobodies, published in Nature.** An LLM "principal investigator" ran a team of LLM scientist agents that designed 92 new nanobodies. Lab tests found working binders against recent variants. [Nature](https://www.nature.com/articles/s41586-025-09442-9)

**Thousands of GPT-Rosalind agents analyzed millions of brain cells in 32 minutes.** They surfaced new leads on neurodegeneration for labs to test. [OpenAI](https://openai.com/index/scaling-ai-research-for-complex-biological-data/)

**A drug discovered with generative AI, both the target and the molecule, has been through a randomized phase 2a clinical trial.** The trial was for idiopathic pulmonary fibrosis and was published in Nature Medicine. [Trial](https://www.nature.com/articles/s41591-025-03743-2) · [Discovery paper](https://www.nature.com/articles/s41587-024-02143-0)

### Other generative AI

**The 2024 Nobel Prize in Chemistry** went partly to AlphaFold. [Nobel Prize](https://www.nobelprize.org/prizes/chemistry/2024/press-release/)

**AlphaFold 3 runs on a diffusion model,** the same kind of architecture as AI art. [Paper](https://www.nature.com/articles/s41586-024-07487-w) · [AlphaFold Server](https://alphafoldserver.com/welcome)

**DeepMind designed enzymes from scratch that do chemistry nature doesn't,** using a diffusion model, then tested them in a real lab. [Preprint](https://www.biorxiv.org/content/10.64898/2026.10.01.756017v1)

**MIT used generative AI to design new compounds that kill drug-resistant bacteria.** [MIT News](https://news.mit.edu/2025/using-generative-ai-researchers-design-compounds-kill-drug-resistant-bacteria-0814)

**An AI-designed drug candidate got IND approval for human trials.** [Article](https://www.drugdiscoverytrends.com/ind-approval-ai-designed-usp1-inhibitor/)

**AI-assisted brain surgery on a real patient.** [BBC](https://www.bbc.co.uk/news/articles/cjwg5n7y68xo)

**Weather forecasting.** [WeatherNext](https://deepmind.google/science/weathernext/)

---

## Coding and cybersecurity

**OpenAI swept the AtCoder World Tour Finals.** Competing alongside the human finalists in the algorithm final, it solved all 5 problems for 8,300 points. The best human scored 4,300, and no human solved two of the problems at all. That means it beat Gennady Korotkevich, the greatest competitive programmer in the world, by at least 4,000 points. It finished first in the heuristic final too. You can't google solutions to brand-new problems mid-contest. [The Decoder](https://the-decoder.com/openais-ai-beats-every-human-at-atcoder-a-top-competitive-programming-contest/) · [MLQ](https://mlq.ai/news/openais-ai-sweeps-all-five-problems-at-atcoder-world-tour-finals-beating-every-human/)

**6,157 real vulnerabilities in 591 open-source projects** reported through Anthropic's disclosure program, as of October 2, 2026. These are real bugs in real software, not benchmarks. [Dashboard](https://red.anthropic.com/2026/cvd/)

**Mythos Preview found previously unknown bugs in every major operating system and browser,** including a 27-year-old bug in OpenBSD, an OS famous for its security. [Anthropic](https://red.anthropic.com/2026/mythos-preview/)

**This isn't locked inside one company.** GLM-5.3 shows similar capabilities, and it's open weights: you can download it and run it on your own hardware. [Anthropic's report](https://www.anthropic.com/research/glm-5-3-and-the-spread-of-advanced-cyber-capabilities) · [Model](https://huggingface.co/zai-org/GLM-5.3) · [OpenAI's report](https://openai.com/index/path-to-astra/)

---

## More papers

Peer-reviewed work using generative AI, by field.

**Biology and medicine:** [Nature Machine Intelligence](https://www.nature.com/articles/s42256-026-01298-6) · [Nature Communications](https://www.nature.com/articles/s41467-026-76760-5) (Chai-1 with ESM protein language model embeddings) · [Nature](https://www.nature.com/articles/s41586-025-10097-9) (a system "powered by large language models") · [Science](https://www.science.org/doi/10.1126/science.aec2657) · [Nature Medicine](https://www.nature.com/articles/s41591-025-04042-6) · [Nature](https://www.nature.com/articles/s41586-025-09298-z) · [Nature](https://www.nature.com/articles/s41586-025-09721-5) · [Mayo Clinic (CNN)](https://edition.cnn.com/2026/07/16/tech/mayo-clinic-ai-healthcare)

**Physics:** [PRX Intelligence](https://journals.aps.org/prxintelligence/abstract/10.1103/9qlr-jp6x) · [PRX Intelligence](https://journals.aps.org/prxintelligence/abstract/10.1103/dldf-7tfm) (diffusion) · [Nature Communications](https://www.nature.com/articles/s41467-024-49104-4) · [EPJ C](https://link.springer.com/article/10.1140/epjc/s10052-024-13701-w) (GANs) · [Physical Review C](https://journals.aps.org/prc/abstract/10.1103/nmmz-bwcs) (diffusion) · [Nature Communications](https://www.nature.com/articles/s41467-026-72292-0) · [Nature](https://www.nature.com/articles/s41586-026-10952-3)

---

## Why this matters everywhere

All of this intelligence transfers. LLMs aren't like specialists who get a degree in one or two fields; they do everything. Being good at math doesn't just mean doing math. It means being very good at logical reasoning in general, and that carries over to coding, biology, chemistry, engineering, and more.
