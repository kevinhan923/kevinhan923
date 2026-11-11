## Mengcheng (Kevin) Han

Computer science senior at New York University (B.A. expected December 2026).
I do research in natural language processing: how machine translation holds up on noisy real-world text, and how retrieval systems should be evaluated. Before that I worked on incentive design for mobile crowdsensing.

### Research

**CCN-MTBench: the cost of conventionalized noise in Chinese→English social-media translation**
First author, team of four · research program mentored by Prof. Philipp Koehn (Johns Hopkins University) · paper under review

- A clean-vs-noisy benchmark of 759 minimal pairs. Each pair differs only inside one annotated span: a homophone respelling, a pinyin initialism, an internet neologism, or embedded English.
- All 18 translation systems we tested, from Qwen3-0.6B to GPT-4o, Gemini and DeepSeek, get significantly worse on the noisy side (27,324 scored translations). Homophones cost the most, although they change fewer than two characters on average.
- Repair with gold spans shows the headroom is real. Our own noise detector does not reach it: it can locate noise but cannot restore the intended form.
- Data, every system output, and code: [kevinhan923/ccn-mtbench](https://github.com/kevinhan923/ccn-mtbench)

**One Vector Is Enough: A Controlled Comparison of Document- and Paragraph-Level Retrieval**
Sole author · NLPVR 2026 (accepted)

- Two-stage pipelines report that scoring paragraphs is worse than encoding a whole document as one vector. I reran the comparison so that both systems share one encoder configuration and rank the full corpus.
- Under that control the penalty disappears: no difference on any of the five corpora survives Holm correction. With the two-stage vectorizer, paragraph-level retrieval is significantly better on NFCorpus and SciFact.
- Along the way I found and repaired three evaluation defects, including a query-numbering mismatch in Cranfield that had offset 152 queries from their relevance judgments.
- Code and result files: [kevinhan923/NLP_IR_Representation_Project](https://github.com/kevinhan923/NLP_IR_Representation_Project)

**Lifecycle-aware incentive pricing for time-sensitive mobile crowdsensing**
First author, with Prof. Jun Tao (Southeast University) · manuscript in preparation

- A two-stage Stackelberg model of long-term incentives, checked against OpenStreetMap contribution history (96,870 contributors over 257 months).

**Also**

- Third author on two manuscripts under review: dataflow analysis of lightweight IoT authentication protocols, and zero-knowledge data-quality proofs for crowdsensing.
- First author of a MoWiN 2022 paper on license-plate detection from a phone photo ([doi:10.5121/csit.2022.120406](https://doi.org/10.5121/csit.2022.120406)).

### About this account

Most of my repositories hold manuscripts that are still under review, so they are private. The public ones are released artifacts.

### Links

[hanmengcheng.com](https://hanmengcheng.com) · [LinkedIn](https://www.linkedin.com/in/mengchenghan)
