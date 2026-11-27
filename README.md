# AI Achievements

Everything here is generative AI: LLMs and other transformers, diffusion models, and GANs. Same family of tech as chatbots and "AI art."

*Last updated November 28, 2026.*

---

## Start here

If you only open seven links, open these. Each one has someone outside the AI company vouching for it.

1. **The Riemann Hypothesis (open since 1859) is proved, and the people who run Lean certified it.** Levent Alpöge, a mathematician at Anthropic, released the proof he found with Claude on November 20, 2026, as a 17-million-line Lean library. The next day, the Lean FRO and the Mathlib Initiative, the groups behind the Lean proof checker and its math library, put out a joint statement: "We hereby certify that both the statement and the proof of the Riemann Hypothesis are correct." Dozens of people rebuilt it themselves, and several independently written proof checkers accepted it. It proves the Generalized Riemann Hypothesis for Dirichlet L-functions too. In Alpöge's words, "Claude far outpaced me near the finish line." There's no human-readable paper yet, so mathematicians still have to digest the ideas, but a machine has checked every step. [Announcement](https://alpo.ge/remark.pdf) · [Lean FRO + Mathlib statement](https://leanprover-community.github.io/blog/posts/riemann-hypothesis/) · [Independent check (Waterloo)](https://www.math.uwaterloo.ca/~mrubinst/alpoge_claude_grh/)

2. **The KLS conjecture (open since 1995) is proved, and the experts credit ChatGPT.** Bizeul, Klartag and Lehec, the people who made the previous big progress on this exact problem, say in their own paper that most of the proofs and ideas in it were found by ChatGPT. [Paper](https://arxiv.org/abs/2610.05474)

3. **An 80-year-old Erdős conjecture disproved, and Fields Medalist Tim Gowers says he'd have accepted it into the Annals of Mathematics.** An OpenAI model disproved the unit distance conjecture in one shot. Nine outside mathematicians checked it, and Gowers wrote he "would have recommended acceptance without any hesitation." [OpenAI](https://openai.com/index/model-disproves-discrete-geometry-conjecture/) · [Mathematicians' paper](https://arxiv.org/abs/2605.20695)

4. **The Jacobian conjecture (open since 1939) is false, and you can check it with a calculator.** Mathematician Levent Alpöge and Claude found a counterexample short enough to fit in a tweet. Terence Tao checked it, and it's been formally verified in Isabelle. [Wikipedia](https://en.wikipedia.org/wiki/Jacobian_conjecture#Counterexample_for_n_%3E_2) · [Formal verification](https://isa-afp.org/entries/Jacobian_Counterexample.html)

5. **Claude broke a physics record, and the record holder verified it himself.** Claude computed a scattering amplitude at nine loops, one past the eight-loop record SLAC's Lance Dixon set in 2023. Dixon checked it. [Anthropic](https://www.anthropic.com/research/yes-claude-can-do-nine-loops)

6. **Google's AI-built flu forecaster beat the CDC's own forecast.** It ranked #1 of 39 models in the CDC's 2025–26 season evaluation. The CDC's official ensemble came 7th. The forecasts were made before the outcomes were known, and the CDC did the scoring. [Google](https://blog.google/innovation-and-ai/models-and-research/google-research/google-science-ai-flu-forecasts/)

7. **The Erdős–Szemerédi sunflower conjecture (from 1978) is proved, and the mathematicians credit ChatGPT with the key argument.** [Paper](https://arxiv.org/abs/2610.26686)

---

## Mathematics

**The Riemann Hypothesis:** see Start here.

**The sunflower conjecture of Erdős and Rado (from 1960).** It says that any big enough family of small sets must contain a "sunflower": several sets that all overlap in exactly the same core. It's one of the best-known open problems in combinatorics. Humans made a big breakthrough on it in 2019 but still couldn't finish it. On November 24, 2026, OpenAI posted a proof of the conjecture for every fixed number of petals. [Paper](https://github.com/openai/math/blob/main/preprints/An-exponential-bound-for-sunflowers-November-24-2026/paper.pdf)

**The Courtade–Kumar conjecture (from 2013), proved and checked in Lean.** It's a basic question in information theory: if you send bits through a noisy channel and can keep only one bit's worth of summary, what's the best summary? The conjecture says just copying one input bit is the best you can do. Researchers from Google, CUHK, USC and CMU, working with Gemini 4 agents in Google's Antigravity, proved it in full generality, and the proof was formalized in about 50 million lines of Lean. The same system also formalized Deligne's 1974 proof of the Weil conjectures, about 1.8 million lines of Lean. [Interesting Engineering](https://interestingengineering.com/ai-robotics/google-antigravity-multi-agent-research)

**The Köthe conjecture (from 1930), disproved by an AI with nobody steering it.** A ring-theory problem open for 96 years. Epoch AI, an outside evaluation organization, turned a pre-release GPT-6 Astra loose on a list of open problems in its own harness, with no human guidance, and it came back with an explicit counterexample and a Lean proof of it. Ring theorists have since written their own papers on it. Nobody prompted it toward the answer; it was handed a list and found one. [Lean disproof](https://github.com/tadamcz/koethe) · [Mathematicians' paper](https://arxiv.org/abs/2609.15080) · [Wikipedia](https://en.wikipedia.org/wiki/K%C3%B6the_conjecture)

**The Unique Games conjecture, and a race that says a lot.** It's widely called the second most important open problem in complexity theory after P vs NP. In September 2026, word got around that OpenAI was about to announce a proof. MIT's Dor Minzer and two of his students rushed out a 95-page paper on a related problem to get ahead of it. On October 6, OpenAI published its proof, with a Lean certificate, as one of 377 results dropped at once. Scott Aaronson wrote that "we're pretty sure that it's a proof." Human mathematicians are now racing machines to their own open problems. [Quanta](https://www.quantamagazine.org/as-ai-closed-in-on-unique-games-proof-researchers-raced-to-beat-the-machines-20261007/) · [Paper](https://github.com/openai/math/blob/main/preprints/The-Unique-Games-Theorem-September-23-2026/paper.pdf)

**A Millennium Prize problem: Navier–Stokes.** About 10,000 OpenAI agents worked for 88 hours and produced a proof that the 3D Navier–Stokes equations can blow up in finite time, formalized in Lean. Quanta Magazine's headline: "AI Has Solved One of Math's $1 Million Millennium Prize Problems." [OpenAI](https://openai.com/index/navier-stokes-solution/)
In November, it went further. Anthropic's Levent Alpöge and NYU's Tristan Buckmaster posted a claim of blow-up with no external force at all, with a 600,000-line Lean formalization. That's the clean version of the problem, with nothing pushing the fluid. One numerical certificate it depends on hasn't been released yet, so treat this one as a fresh claim rather than a settled result. [Report](https://officechai.com/ai/tristan-buckmaster-levent-alpoge-claim-proof-of-navier-stokes-millennium-prize-problem-without-forcing/)

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

**VP ≠ VNP, the algebraic version of P vs NP, from two AI labs on the same day.** In 1979, Leslie Valiant conjectured that the permanent, a close cousin of the determinant, can't be computed by any small circuit of additions and multiplications. On November 23, 2026, Anthropic and OpenAI each posted an AI-made proof, about four hours apart, and both come with Lean formalizations. Anthropic's 70-page paper lists Claude as its only author. The next day, OpenAI went further and separated the whole hierarchy of circuit classes. Anthropic says no human mathematician has checked its proof yet, so for now the Lean check is what vouches for it. It doesn't settle P vs NP itself. [Anthropic paper + Lean proof](https://github.com/anthropics/formal-math/tree/main/vp-vnp) · [OpenAI paper](https://github.com/openai/math/blob/main/preprints/VP-and-VNP-are-different-November-23-2026/paper.pdf) · [OpenAI's stronger follow-up](https://github.com/openai/math/blob/main/preprints/Paths-trees-and-grids-separate-Valiants-hierarchy-November-24-2026/paper.pdf) · [Independent Lean re-check](https://github.com/Horace-Maxwell/vp-vnp-lean-independent-verification)

**Smale's ninth problem: linear programming in strongly polynomial time.** Linear programming runs logistics, scheduling and much of operations research. In 1998, Steve Smale put it on his list of the biggest math problems for the 21st century: can it be solved in a number of steps that depends only on the size of the problem, not on how big the numbers in it are? On November 24, 2026, OpenAI posted a deterministic algorithm that does exactly that, with the rational-number case checked in Lean. A companion paper disproves the polynomial Hirsch conjecture: some polytopes have corners that are superpolynomially many edges apart, which means no version of the classic simplex method could ever have been the answer. Both are new and not yet reviewed by outside experts. [Paper](https://github.com/openai/math/blob/main/preprints/Strongly-polynomial-linear-programming-November-24-2026/paper.pdf) · [Hirsch paper](https://github.com/openai/math/blob/main/preprints/Superpolynomial-graph-diameter-of-simple-polytopes-November-24-2026/paper.pdf)

**Six math papers in a single day, from one prompt each.** On November 25, 2026, Google Research dropped six papers written entirely by Cogentic, its multi-agent system running on Gemini 4, each with a Lean 4 formalization. The headline one closes a gap open since 1992: an unconditional algorithm that factors any integer in subexponential expected time, with no unproven assumptions and no chance of a wrong answer. The others cover discrete logarithms, Nash equilibria, the log-rank conjecture and edge reconstruction. Google says there was no human involvement beyond the initial prompt. Nobody outside Google has checked them yet, and to be clear, this does not break RSA. [Papers](https://github.com/google-research/google-research/tree/master/cogentic_research_papers)

**The Exponential Time Hypothesis is false.** Since 1999, ETH said 3-SAT can't be solved meaningfully faster than exponential time, and Claude's literature search found over 800 papers built on it or on something stronger. On October 16, 2026, an OpenAI model and a Claude model each independently found a subexponential algorithm, on the same day. Both are formalized in Lean, and the people who proposed ETH are running the review themselves. [OpenAI paper](https://github.com/openai/math/blob/main/preprints/The-Exponential-Time-Hypothesis-is-False-October-25-2026/paper.pdf) · [Anthropic paper + Lean proof](https://github.com/anthropics/formal-math/tree/main/eth)

**The matrix multiplication exponent is exactly 2.25, settling a question open since 1969.** Multiplying matrices is the core operation behind basically all of modern computing, AI included, and the exponent ω measures how fast that work grows. In 1990, Coppersmith and Winograd got it down to 2.3755. Over the next 35 years, the best people in the field moved it to 2.3713, less than 0.005 in total. In October 2026, an internal OpenAI model proved ω ≤ 9/4 = 2.25, nearly 30 times all that progress in one jump, with the main theorem checked in Lean. Mathematician Steven Strogatz compared it to "Bob Beamon's long jump," and mathematicians at LMU Munich have since reworked that proof independently and formalized it in Lean themselves. Then on November 24, OpenAI posted the matching lower bound: no method can beat 2.25, over any field. So the exponent is exactly 9/4, and the popular guess that it's 2 is wrong. The lower bound is checked in Lean for division-free circuits. [Upper bound](https://github.com/openai/math/blob/main/preprints/Matrix-Multiplication-Nine-Fourths-October-2-2026/paper.pdf) · [Lower bound](https://github.com/openai/math/blob/main/preprints/The-matrix-multiplication-exponent-is-nine-fourths-November-24-2026/paper.pdf) · [Lean proof](https://github.com/openai/math/tree/main/lean/OAI/LinearAlgebra/MatrixMultiplication)

**Truly subquadratic 3SUM and truly subcubic APSP.** The 3SUM and APSP hypotheses are two of the central "you can't go faster than this" assumptions of fine-grained complexity, and this paper by Josh Alman and Virginia Vassilevska Williams beats both. The paper says an Anthropic employee used an internal research model to investigate open problems in the theory of cryptography, and Anthropic released a Lean formalization of the results. It looks incremental, but it's like finding out you can go 1.000004x the speed of light: tiny on paper, but the wall was supposed to be unbreakable. [Paper](https://arxiv.org/html/2610.06783v1#Sx1.SS0.SSS0.Px1) · [Lean formalization](https://github.com/anthropics/formal-math/tree/main/3sum-apsp)

**The Aaronson–Ambainis conjecture (open since 2008) is proved, and the proof is checked in Lean.** It's one of the central open problems in quantum computing: it says exponential quantum speedups need structure, and that on almost all inputs a classical algorithm can approximate a quantum one with only polynomially more queries. In 2019, two mathematicians announced a proof, and it turned out to have a subtle flaw. Physical Superintelligence's research system, running instances of an unreleased Anthropic model, wrote down a complete proof on the third day of its run, then pushed the bound's exponent from 22 down to 7. Lean's kernel checked it with no unproven assumptions, and Scott Aaronson himself pointed PSI to a team of complexity theorists who are writing up an exposition of the proof for experts. [Paper](https://github.com/physical-superintelligence/aaronson-ambainis/blob/main/paper/aaronson_ambainis_paper.pdf) · [Lean proof](https://github.com/physical-superintelligence/aaronson-ambainis) · [The flawed 2019 attempt](https://arxiv.org/html/2402.13952v2)

---

## Physics

**Yang–Mills existence, half of a Millennium Prize problem.** OpenAI's model produced a rigorous existence proof for pure Yang–Mills theory in 4 dimensions, then for QCD, the theory of quarks and gluons. Physicists have used these theories for decades without a proof that they mathematically exist. On November 10, 2026, a five-member committee chaired by Nobel laureate David Gross, including Arthur Jaffe, who co-wrote the official Millennium Prize problem statement, published OpenAI's Lean code with an assessment confirming that pure Yang–Mills theory exists in 4 dimensions. The mass gap half is still open. [Lean code](https://github.com/yang-mills-group/OpenAI-YM-20261028) · [Background](https://en.wikipedia.org/wiki/Yang%E2%80%93Mills_existence_and_mass_gap)

**Claude solved two open problems about black holes.** One was a calculation laid out in 2003 and never finished: whether a quantum version of the Hawking–Page black hole transition is sudden or smooth. Claude showed it's sudden. The other was how tightly the "modular bootstrap" can bound the mass of the lightest black hole in 3D gravity. The best proven bound was c/8.5; Claude derived an exact formula, pushed it to about c/9.13, and proved that's the best this method can ever give, with the results checked in Lean. Claude Fable 5.2, a model anyone can use, ran a small research group of copies of itself for about six weeks and wrote the papers with minimal guidance. [Anthropic](https://www.anthropic.com/research/claude-black-hole-physics) · [Paper 1](https://hexagonmath.org/2611.00175v1) · [Paper 2](https://hexagonmath.org/2611.00174v1)

**49 of 50 unpublished research-level physics problems.** Physicists wrote 50 brand-new problems that take an expert a day or more each. GPT-6 Astra got 49 right at under $3 per problem. At first it scored lower, because in several cases it insisted the experts' answer keys were wrong. It was right. [Paper](https://arxiv.org/abs/2610.16733)

**Nine loops:** see Start here. [Anthropic](https://www.anthropic.com/research/yes-claude-can-do-nine-loops)

---

## Medicine, chemistry and biology

### LLMs

**AI beat doctors at diagnosis in Science.** On real emergency-room cases at the first decision point, OpenAI's o1 got the correct or near-correct diagnosis about 67% of the time, versus 50–55% for expert physicians. [Paper](https://www.science.org/doi/10.1126/science.adz4433)

**Microsoft's AI was more than twice as accurate as doctors, in Science.** Instead of being handed a finished case file, MAI-DxO works a case the way a doctor does: asking questions, ordering tests, narrowing down. On 304 of the hardest case records from the New England Journal of Medicine, it reached the right diagnosis 83.2% of the time. Generalist physicians with textbooks and the internet got 36.1%. Published in Science (vol. 394, pp. 423–428), October 22, 2026. [Paper](https://www.microsoft.com/en-us/research/publication/sequential-diagnosis-with-language-models/) · [Coverage](https://thenextweb.com/news/microsoft-ai-diagnosis-mai-dxo-science-study)

**18 new rare-disease diagnoses that years of specialists couldn't crack.** Doctors used OpenAI's o3 on 376 previously unsolved rare-disease cases. The model surfaced the leads, and every diagnosis was confirmed clinically. [OpenAI](https://openai.com/index/diagnose-rare-childhood-diseases/) · [NEJM AI paper](https://ai.nejm.org/doi/full/10.1056/AIcs2501343?query=featured_home)

**Claude found a new CRISPR-like enzyme system.** About 950 Claude agents searched more than 200,000 enzymes in 21 hours and spotted a system nobody had recognized. CRISPR pioneer Feng Zhang called the connection "genuinely intriguing." Nobody knows yet what it does. [Anthropic](https://www.anthropic.com/news/claude-discovers-novel-enzyme-system)

**Claude designs proteins as well as top human experts.** It designed binders against 14 of 15 targets, with hit rates over 20% versus the typical 10–15%. Independent labs built and tested the designs. [Anthropic](https://www.anthropic.com/research/Claude-accelerates-protein-design)

**Claude designed proteins against scorpion toxins.** It worked mostly on its own for 64 hours. Independent labs tested 211 designs, and 17 bound their targets. [Anthropic](https://www.anthropic.com/research/claude-scorpion-toxin-binder-design)

**GPT-6 designs proteins with nothing but reasoning and code.** Protein design is normally done by specialized models like RFdiffusion. OpenAI showed its general-purpose GPT-6 models can design protein shapes and sequences themselves, by thinking and writing ordinary code. In lab tests run by its partner Onava, proteins based on GPT-6.2's designs bound all five targets they were aimed at, and when it redesigned sequences for one target, MDM2, 75 of 88 bound (85%). Specialized models still helped filter the candidates, and it hasn't been peer-reviewed yet. [OpenAI](https://openai.com/index/gpt-6-models-demonstrate-intrinsic-protein-design-capabilities/)

**Claude helped get the first 3D structure of a vault particle found in bacteria.** Vaults are giant hollow protein shells found in our cells, and nobody has figured out what they do since they were discovered in 1986. Anthropic's biologists, with Claude doing every major research step, found vaults made by viruses that infect bacteria and imaged one: a shell of 96 copies of one protein, among the largest protein shells ever found in bacteria. Claude searched 15 billion predicted proteins, designed the DNA, and ran the cryo-electron microscopy processing; it had a first 3D model 34 hours after processing began. Leonard Rome, who co-discovered vaults, advised on the work. [Anthropic](https://www.anthropic.com/research/investigating-vault-particles-with-claude) · [Preprint](https://www.biorxiv.org/content/10.64898/2026.11.04.764334v1)

**GPT-5 made a lab technique 79x more efficient.** It improved a standard molecular cloning protocol over several rounds of real lab experiments, introducing a mechanism of its own. [OpenAI](https://openai.com/index/accelerating-biological-research-in-the-wet-lab/)

**A lab run by LLM agents, published in Nature.** AutoDNA's agents coordinate 20+ kinds of lab instruments and have run more than 11,000 experimental steps, matching results that human experts published. [Nature](https://www.nature.com/articles/s41586-026-11228-6)

**A team of AI scientists designed new COVID nanobodies, published in Nature.** An LLM "principal investigator" ran a team of LLM scientist agents that designed 92 new nanobodies. Lab tests found working binders against recent variants. [Nature](https://www.nature.com/articles/s41586-025-09442-9)

**Thousands of GPT-Rosalind agents analyzed millions of brain cells in 32 minutes.** They surfaced new leads on neurodegeneration for labs to test. [OpenAI](https://openai.com/index/scaling-ai-research-for-complex-biological-data/)

**An AI "virtual scientist" designed working RNA molecules, in Nature Biotechnology.** RhoAgent, from a CUHK-led team, takes a plain-language design request, generates RNA with a diffusion model, and improves its designs using feedback from real lab experiments. It built functional ribozymes, RNA molecules that act as enzymes, and made one of them cut its target up to six times more efficiently than the human-expert version. Peer-reviewed, with the lab work actually done. [Nature Biotechnology](https://www.nature.com/articles/s41587-026-03362-3)

**A drug discovered with generative AI, both the target and the molecule, has been through a randomized phase 2a clinical trial.** The trial was for idiopathic pulmonary fibrosis and was published in Nature Medicine. [Trial](https://www.nature.com/articles/s41591-025-03743-2) · [Discovery paper](https://www.nature.com/articles/s41587-024-02143-0)
It's now in Phase III. On September 9, 2026, Insilico Medicine dosed the first patient in GENESIS-IPF-3, the first late-stage trial anywhere of a drug whose target and molecule both came from generative AI. [Announcement](https://www.prnewswire.com/news-releases/insilico-medicine-doses-first-patient-in-genesis-ipf-3-the-worlds-first-phase-iii-trial-of-a-generative-ai-driven-innovative-drug-302873749.html)

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

**Claude rebuilt a 16,000-line program without ever seeing its source code.** In MirrorCode, a benchmark from Epoch AI and METR, a model gets to run a program, read its documentation and check itself against tests, but never sees a line of the original code, and has to reimplement it exactly. Claude Opus 4.7 rebuilt gotree, a bioinformatics toolkit with about 16,000 lines of Go and 40+ commands, in 14 hours for $251. Epoch and METR estimate the same job would take a human engineer 2 to 17 weeks. [Epoch AI paper](https://epoch.ai/files/MirrorCode.pdf) · [The Decoder](https://the-decoder.com/an-ai-model-programmed-nonstop-for-19-days-on-a-single-mirrorcode-task-that-cost-2600-to-run/)

**Claude built a working operating system from an empty folder.** In an Anthropic experiment, one engineer gave Claude Fable 5.2 a basic prompt and an empty project folder. Over eight days it coordinated more than 1,000 agents and produced a prototype operating system that boots on a laptop, with its own kernel, disk, keyboard and network drivers, file storage, windows, a login screen and an installer. Building an operating system is one of the hardest projects in software, and Fable 5.2 is a model anyone can use today. [Anthropic](https://www.anthropic.com/claude-fable-and-mythos-5-2) · [Interesting Engineering](https://interestingengineering.com/ai-robotics/anthropic-claude-fable-5-2-operating-system)

**Claude designed three real electronic gadgets that worked on the first build.** From short prompts, Claude Fable 5.2 designed a USB speakerphone, a voice-assistant hub and a handheld virtual pet: the specs, circuit schematics, board layouts, enclosures, firmware and parts lists. Diode Computers manufactured the boards straight from Claude's files, and all three worked without any fixes to their circuitry, and were still working weeks later. They're early prototypes that haven't been through certification testing. [Anthropic](https://www.anthropic.com/research/claude-electronics-design)

**AI agents proved Signal's security down to the machine code.** Google DeepMind's AlphaProof Code had Gemini-powered agents write about 6.5 million lines of machine-checked Lean proof, showing that the compiled code behind Signal's one-to-one chats actually has the security properties it's supposed to: forward secrecy, post-compromise security and authentication. Verifying real cryptographic code this deep has traditionally taken teams of experts years. Five researchers did it in four weeks, and Signal's CTO said it gives them "even greater confidence in our code's privacy guarantees." [The Register](https://www.theregister.com/ai-and-ml/2026/11/10/google-deepmind-melds-humans-and-ai-agents-to-vet-signals-secure-messaging-techniques/5308625) · [Lean proofs](https://github.com/google-deepmind/code-verification)

**AI-written code has been running Google's data centers for over a year.** AlphaEvolve, a Gemini-powered coding agent, wrote a scheduling algorithm that continuously recovers 0.7% of Google's worldwide compute. It sped up a key kernel in Gemini's training by 23%, cutting Gemini's total training time by 1%, so the AI is speeding up the training of the models it runs on. It also found a way to multiply 4×4 complex matrices with 48 multiplications, beating Strassen's 1969 record of 49 for the first time in 56 years. [Google DeepMind](https://deepmind.google/discover/blog/alphaevolve-a-gemini-powered-coding-agent-for-designing-advanced-algorithms/)

**AlphaDev found faster sorting algorithms, and they're in the C++ standard library.** DeepMind's system discovered sorting routines faster than the ones human engineers had refined for over a decade. They were merged into LLVM's libc++, the first change to those algorithms in more than ten years. Sorting is called trillions of times a day, so this is AI-discovered code running under an enormous amount of the world's software. [Nature](https://www.nature.com/articles/s41586-023-06004-9)

**Agents built a graph system that handles 1.14 trillion edges.** Google's Graph Mining team used Gemini 4 Argon agents in Antigravity to write FarArray, which runs graph algorithms over 18 billion vertices and 1.14 trillion edges. Google reports 40–180x faster runtimes than the baselines it replaces and over 100x less cluster memory, and says the agents compressed months of low-level RDMA networking and TPU kernel work into hours. [Google](https://antigravity.google/blog/gemini-4-argon-trillion-edge-graphs-and-tpu-kernels)

**AI systems won DARPA's $4 million AI Cyber Challenge.** In the final round, autonomous systems built on LLMs like o3 and GPT-4o hunted through 54 million lines of real open-source code. They found 54 of the vulnerabilities DARPA had planted and patched 43, taking about 45 minutes per patch on average, and found 18 real vulnerabilities nobody had planted. This one was run and scored by DARPA, not an AI company. [DARPA](https://darpa.mil/news/2025/aixcc-results)

**6,157 real vulnerabilities in 591 open-source projects** reported through Anthropic's disclosure program, as of October 2, 2026. These are real bugs in real software, not benchmarks. [Dashboard](https://red.anthropic.com/2026/cvd/)

**Earlier milestones worth remembering.** In 2024, Google's Big Sleep agent found a previously unknown exploitable bug in SQLite, one of the most widely deployed and most heavily tested pieces of software on earth, before it ever shipped. In 2025, DeepMind's CodeMender landed 72 security fixes in open-source projects. These were the early versions of what the entries above have become. [Big Sleep](https://googleprojectzero.blogspot.com/2024/10/from-naptime-to-big-sleep.html) · [CodeMender](https://deepmind.google/blog/introducing-codemender-an-ai-agent-for-code-security/)

**Claude found 22 Firefox vulnerabilities in two weeks, and Mozilla confirmed every one.** Working with Mozilla, Claude Opus 4.6 found 22 security bugs that got official CVEs, 14 of them rated high severity. That's almost a fifth of all the high-severity Firefox vulnerabilities fixed in the whole of 2025. Mozilla patched them, along with about 90 more non-security bugs Claude reported. [Axios](https://www.axios.com/2026/03/06/anthropic-mozilla-claude-opus-bug-hunting) · [TechCrunch](https://techcrunch.com/2026/03/06/anthropics-claude-found-22-vulnerabilities-in-firefox-over-two-weeks/)

**GPT-6 Cyber found 81 new high-severity Firefox flaws and built working root exploits for 948 Linux kernel bugs.** Mozilla rated all 81 Firefox bugs high severity and has been shipping the fixes, in what Mozilla's Brian Grinstead called one of the most hardened codebases going into 2026. On the Linux kernel, the model reproduced 1,724 vulnerabilities and wrote working privilege-escalation exploits for 948 of them, more than five times the 166 its predecessor GPT-5.6 Sol managed in the same setup. [BleepingComputer](https://www.bleepingcomputer.com/news/security/openais-new-gpt-6-cyber-ai-finds-81-firefox-flaws-948-linux-bugs/)

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
