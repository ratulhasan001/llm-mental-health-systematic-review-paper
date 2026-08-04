# 1. Review Methodology and the Secondary Evidence Base

## 1.0 Purpose and placement

This chapter opens with the secondary literature rather than with primary studies, for two reasons. First, ten of the sixty-six studies in the corpus (15.2%) are themselves reviews, surveys, or conceptual syntheses; they are evidence *about* the field's methodology rather than instances of it, and reading them first establishes the vocabulary the remaining fifty-six papers are described in. Second, a methodology review must justify its own existence. Seven systematic or scoping reviews of large language models (LLMs) in mental health were published between 2024 and 2026, and any new synthesis has to demonstrate that it addresses something those seven did not. This section establishes both the inherited conceptual apparatus and the specific gap the present review occupies.

The ten papers divide into three methodologically distinct groups: scoping reviews that map breadth (§1.1), systematic reviews conducted under PRISMA that additionally attempt appraisal (§1.2), and conceptual or position papers that supply taxonomies and governance frameworks without primary data (§1.3).

---

## 1.1 Scoping reviews: mapping the application landscape

Four studies adopt a scoping design, whose explicit aim is coverage rather than effect estimation.

**Jin et al. (2025)** conducted the broadest search in the corpus by database count, querying seven electronic databases — Web of Science, PubMed, Cochrane Library, IEEE Xplore, and the Chinese-language databases Weipu, CNKI, and Wanfang — for studies published between 1 January 2019 and 31 August 2024. From 4,859 retrieved records, 95 were included. Two features distinguish this review methodologically. It is prospectively registered on the Open Science Framework, a practice adopted by only two of the seven empirical reviews reviewed here. And its inclusion of three Chinese-language databases makes it the only synthesis in the corpus with systematic non-English coverage, which matters given that a substantial share of primary work in this corpus originates from Chinese institutions. Screening proceeded in three rounds — title/abstract, cross-check, full-text — with disagreements escalated to third reviewers until consensus. Extracted data were synthesised descriptively in R (v4.4.2), with no attempt at pooling.

**Hua et al. (2025a)** searched six sources including three preprint servers (arXiv, medRxiv, PsyArXiv) alongside PubMed, Web of Science, and Google Scholar, covering 1 October 2019 to 2 December 2023, and included 34 of 313 records. The decision to admit non-peer-reviewed preprints is a deliberate trade-off: it reduces the recency lag that afflicts every other review here, at the cost of admitting unrefereed work. The review's most consequential methodological contribution is internal to its own process. GPT-4 was deployed as a parallel screening reviewer alongside a human, with agreement quantified by Cohen's κ (≈0.90). This is the only study in the corpus to treat LLM-assisted evidence synthesis as an object of measurement rather than a convenience, and it is directly relevant to the methods debated in §4.3 on LLM-as-judge reliability.

**Yang et al. (2026)** conducted the largest search by volume, retrieving 10,743 records across eleven databases, assessing 58 at full text, and charting 29. It is the only review to follow both PRISMA-ScR and the Joanna Briggs Institute scoping framework. Screening and charting were performed by two independent reviewers (JY, TL) with a third (YL) resolving discrepancies, and qualitative interpretations were verified by all authors. Its framing is also distinctive: where the other reviews ask what LLMs *can* do, this one asks where their application *boundaries* lie, charting technical, ethical, and practical limits per study. That orientation makes it the closest antecedent to the risk-focused synthesis developed in §6.

**Hua et al. (2025b)** searched four databases (APA PsycNet, Scopus, PubMed, Web of Science) for peer-reviewed work published between 1 January 2020 and 19 July 2024, including 16 of 726 unique articles under PRISMA 2020. Its narrower scope — generative tasks only, defined via a parameter threshold — yields the smallest included set among the scoping reviews. Its methodological value lies in mapping primary studies onto a three-level *clinical evaluation pyramid*, converting a descriptive exercise into a diagnostic one: rather than reporting what studies found, it reports where in a hierarchy of clinical evidence they sit, and shows that the literature clusters at the lowest tier.

---

## 1.2 PRISMA systematic reviews: appraisal and its absence

Three studies adopt a systematic review design, and the differences between them are instructive precisely because the label is shared.

**Wang et al. (2025)** searched five databases (PubMed, Embase, Web of Science, Engineering Village, PsycINFO), screening 1,046 references with paired independent reviewers in Rayyan and including just eight studies. This is the most restrictive inclusion in the corpus — a 0.76% inclusion rate — and it is the only review to apply a formal quality appraisal instrument, the Mixed Methods Appraisal Tool (MMAT, 2018). The review classifies primary research by the *clinical competencies* a human therapist would require (assessment, intervention, cultural humility), which reframes model evaluation around clinical role rather than technical task. Its own stated limitation is severe: with N=8, and with the included studies weighted heavily toward zero-shot prompt tests, its conclusions rest on a thin base and no meta-analysis is attempted.

**Kolding et al. (2025)** searched PubMed, Embase, and PsycINFO, screening 724 unique records after removing 432 duplicates from 1,156, and including 40 studies with a protocol preregistered on the Open Science Framework. Screening was dual-reviewer at both title/abstract and full-text stages, supported by Covidence. Notably, the authors state explicitly that no formal quality appraisal or quantitative synthesis was performed, attributing this to the relative immaturity of the field. This candour is methodologically valuable: it is a documented decision rather than an omission, and it identifies the field's condition — not the reviewers' resources — as the binding constraint. The review's substantive contribution to the present chapter is its finding that models and prompts are so severely underspecified in the published literature that replication is frequently impossible, a claim independently corroborated by the extraction reported in §7.3.

**Guo et al. (2024)** collated 40 peer-reviewed articles from MEDLINE, IEEE Xplore, Scopus, JMIR, and the ACM Digital Library, spanning the widest temporal window of any review here (1 January 2017 – 30 April 2024). It is the only review to apply the Cochrane **Risk of Bias 2** tool to this literature, and one of only two to report inter-reviewer agreement (Cohen's κ = 0.84, with a third reviewer consulted for disagreements). Its conclusion is the most restrictive in the corpus — that current risks of clinical use may outweigh the benefits — and it identifies the absence of a benchmarked ethical framework as a structural gap alongside hallucination and output inconsistency. Its acknowledged limitation is that 98% of the papers it reviewed cover only BERT- and GPT-family models, leaving the wider model landscape unexamined.

**Table 1.1 — Review protocol parameters across the seven empirical reviews**

| Study | Design | Databases | Screened → Included | Search window ends | Dual screening | Quality appraisal | Agreement reported | Pooling |
|---|---|---|---|---|---|---|---|---|
| Jin et al. (2025) | Scoping | 7 (incl. 3 Chinese) | 4,859 → 95 | Aug 2024 | Yes (3 rounds) | No | No | None |
| Hua et al. (2025a) | Scoping | 6 (incl. preprints) | 313 → 34 | Dec 2023 | Human + GPT-4 | No | κ ≈ 0.90 | None |
| Yang et al. (2026) | Scoping (PRISMA-ScR + JBI) | 11 | 10,743 → 29 | Not reported | Yes (2 + adjudicator) | No | No | None |
| Hua et al. (2025b) | Scoping (PRISMA 2020) | 4 | 726 → 16 | Jul 2024 | Yes | No | No | None |
| Wang et al. (2025) | Systematic (PRISMA) | 5 | 1,046 → 8 | Jun 2024 | Yes (paired) | **MMAT** | No | None |
| Kolding et al. (2025) | Systematic (PRISMA, preregistered) | 3 | 724 → 40 | Feb 2024 | Yes (both stages) | Declined, stated | No | None |
| Guo et al. (2024) | Systematic (PRISMA) | 5 | — → 40 | Apr 2024 | Yes (2 + adjudicator) | **RoB 2** | κ = 0.84 | None |

---

## 1.3 Conceptual, taxonomic, and governance contributions

Three papers contribute no primary data and no systematic search, but supply the conceptual instruments the rest of this chapter relies on.

**Huang et al. (2025)** is a survey of hallucination in LLMs, general-domain rather than mental-health-specific, and it is included because it provides the definitional apparatus applied in §6.1. Its contribution is a layered taxonomy separating **factuality** hallucination (contradiction, fabrication) from **faithfulness** hallucination (instruction, context, and logical inconsistency), with root causes mapped across data, training, and inference stages and matched to corresponding detection and mitigation strategies. It also devotes dedicated treatment to the residual hallucination that survives retrieval augmentation — directly relevant to the RAG systems examined in §3.3. Its limitation is that it is a qualitative synthesis of secondary literature running no primary experiments.

**Chung et al. (2023)** is a perspective paper grounded in the authors' own deployment experience, mapping five architectural challenges — hallucination, interpretability, bias, privacy, clinical effectiveness — to practical mitigations. Its most useful move for this chapter is adapting the intrinsic/extrinsic hallucination distinction specifically to *counselling dialogue*: intrinsic hallucination contradicts the dialogue history, extrinsic hallucination cannot be verified against any available input. It further proposes a dual architecture pairing stochastic neural generation with deterministic hard-coded decision-tree overrides for crisis detection, explicitly conceding that hallucination cannot be eliminated within the current paradigm and must therefore be contained. This concession anticipates the guardrail architectures evaluated in §5.3 and §6.3.

**Asman et al. (2025)** is an editorial and policy synthesis framing a theme issue on responsible generative AI in mental health. Its contribution is a governance roadmap integrating a relational *ethics of care* with clinical alliance standards, and a proposed clinical risk assessment questionnaire for patients and developers. Like the other two papers in this subsection, it offers no empirical evaluation; its role here is to supply the normative frame against which the assurance methods in §6 are judged.

---

## 1.4 Methodological appraisal of the secondary evidence base

Read together, the seven empirical reviews exhibit four consistent properties that define the gap addressed by the present work.

**No review performs quantitative synthesis.** All seven synthesise descriptively. This is a defensible response to genuine heterogeneity — the primary literature reports F1, balanced accuracy, AUC, BLEU, ROUGE, κ, ICC, and bespoke Likert instruments, frequently without shared task definitions — but it means no pooled effect estimate for any LLM mental health application currently exists.

**Quality appraisal is the exception, not the norm.** Only two of seven reviews apply a formal instrument (MMAT in Wang et al.; RoB 2 in Guo et al.), and only two report inter-reviewer agreement. Five reviews therefore synthesise studies of unassessed methodological quality, which constrains how far their conclusions about capability can be trusted.

**Inclusion rates are extremely low and highly variable.** Included proportions range from 0.27% (29 of 10,743) to 10.9% (34 of 313) — a fortyfold spread. Since these reviews cover overlapping periods and substantially overlapping topics, the variance reflects differing operational definitions of "LLM" and "mental health application" rather than differing literatures. Wang et al. include eight studies while Jin et al. include ninety-five, from searches whose windows overlap by more than four years.

**Every search window closes before the majority of the present corpus was published.** This is the decisive gap. The latest search end-date among the seven reviews is August 2024 (Jin et al.), with the earliest at December 2023 (Hua et al., 2025a). Within the corpus analysed in this thesis, 45 of 66 studies (68%) were published in 2025 or 2026 (Table 1.2). The existing secondary literature therefore cannot speak to the methodological developments that dominate the current field: multi-turn adversarial safety benchmarking (§6), agentic and simulation-based red teaming (§3.4, §6.4), LLM-as-judge reliability frameworks (§4.3), and preference-optimisation approaches to alignment (§6.1).

**Table 1.2 — Corpus publication years relative to prior review coverage**

| Year | Studies in corpus | Share | Covered by any prior review's search window |
|---|---|---|---|
| 2023 | 4 | 6% | Yes |
| 2024 | 17 | 26% | Partially |
| 2025 | 36 | 55% | No |
| 2026 | 9 | 14% | No |
| **Total** | **66** | **100%** | **32% at most** |

A fifth observation concerns scope rather than rigour. Five of the seven reviews organise around *application areas* — what LLMs are used for. Only Yang et al. (2026), through its boundary framing, and Hua et al. (2025b), through its evaluation pyramid, organise around evaluative adequacy. None organises around methodology as such: how corpora are constructed, how models are adapted, how evaluation is designed, and how risk is assessed. That is the organising principle of the present review.

---

## 1.5 Positioning of the present review

The methodological commitments adopted here follow directly from the appraisal above.

1. **Extraction is methodology-only.** Results are deliberately excluded. Where prior reviews chart what models achieved, this review charts how the achievement was established — the design, protocol, and evaluation apparatus of each study.
2. **Every study is extracted across the same twenty-four fields**, including four dedicated risk fields (hallucination, bias, safety, human evaluation) that no prior review extracts systematically. This permits the corpus-wide statements in §6 and §7 that the existing literature cannot support.
3. **The search window extends through 2026**, capturing the 68% of the corpus that falls outside all prior review coverage.
4. **Absence is recorded as data.** Following the transparency of Kolding et al. in declaring their own non-appraisal, the extraction distinguishes "Not Reported" from "not applicable," so that gaps in the primary literature — 29 of 66 studies reporting no hallucination evaluation method, for example — become findings rather than blanks.
5. **Duplicate versions are consolidated.** Two studies appeared in the retrieved set in both preprint and published form and were merged into single records, giving 66 unique studies from 68 retrieved documents.

Two limitations of the present synthesis should be stated at the outset, consistent with the appraisal standard applied to prior work. First, like all seven reviews examined here, this review performs no quantitative pooling, for the same heterogeneity reason. Second, no formal quality appraisal instrument (MMAT, RoB 2) is applied to included studies; methodological quality is instead characterised through the extraction fields themselves — statistical analysis, human evaluation, and reliability reporting — and appraised cross-sectionally in §7. This is a weaker guarantee than a validated instrument would provide, and it is a deliberate trade-off against extraction depth across twenty-four fields.

---

*Papers in this section:* Jin et al. 2025 (P07); Hua et al. 2025a (P08); Yang et al. 2026 (P20); Hua et al. 2025b (P22); Wang et al. 2025 (P37); Kolding et al. 2025 (P40); Guo et al. 2024 (P66); Huang et al. 2025 (P15); Asman et al. 2025 (P41); Chung et al. 2023 (P67).


---

# 2. Data Foundations and Corpus Construction

## 2.0 Purpose and placement

Section 1 established that the existing secondary literature organises around application areas rather than methodology. This section begins the methodological account proper, and it begins with data because data constraints determine which methods are subsequently available. The recurring criticism of this field — that models are evaluated on social media proxies rather than clinical presentations — is usually stated as a limitation. Read across twelve studies whose primary contribution is a corpus or an annotation protocol, it is better understood as a structural condition: clinical mental health data is scarce, legally encumbered, and small, and almost every downstream methodological choice examined in Sections 3 to 6 is a response to that scarcity.

Twelve of the sixty-six studies (18.2%) are grouped here because their principal methodological contribution is the construction, integration, or annotation of a dataset, rather than a modelling technique applied to an existing one. They divide into corpora derived from clinical encounters (§2.1), corpora derived from public social platforms (§2.2), synthetically generated corpora (§2.3), and studies whose contribution is the annotation protocol itself (§2.4). Section §2.5 draws out the cross-cutting consequence: a hierarchy of ground-truth provenance that governs how confidently any result in this thesis can be interpreted.

---

## 2.1 Clinical and interview corpora

Four studies work with data generated inside a clinical or semi-clinical encounter. They are the smallest group in this section and, with one exception, the smallest datasets.

**Ohse et al. (2024)** collected the KID corpus of German semi-clinical interviews, transcribed and translated with OpenAI Whisper large-v2, with patient-only utterances extracted manually. DAIC-WOZ and Extended DAIC were used for fine-tuning, making this simultaneously a corpus contribution and a generalisation test: models trained on the established benchmark were evaluated on newly collected data from a different language and protocol. Ground truth was PHQ-8 self-report, dichotomised at the conventional cut-off (≥10) for classification and retained continuously for severity estimation, evaluated by Pearson correlation and mean squared error. The study's own stated limitations are instructive for the section as a whole — a unimodal text approach discarding prosodic and visual cues, manual speaker annotation, translation-induced loss of nuance, and age/gender imbalance in recruitment.

**Sood et al. (2023)** addressed data scarcity directly by construction, integrating DAIC, E-DAIC, and the Chinese-language EATD corpus into a single resource, I-DAIC. The integration required machine translation of EATD via the M2M 1.2B multilingual model, and — significantly — the translated output was validated by human annotators proficient in both English and Chinese, making this the only cross-lingual corpus merge in the corpus with a documented translation-verification step. The study's substantive methodological contribution is a comparative benchmark of five strategies for handling documents that exceed transformer context limits: base truncation, customised truncation retaining the middle 512 tokens, sliding windows with averaged predictions, and extractive summarisation by word count or word frequency. Its most useful negative finding is that fine-tuned BERT and RoBERTa underperformed TF-IDF-based SVM and logistic regression on weighted F1, which the authors attribute to severe class imbalance — a result that should temper any assumption that transformer adaptation is automatically superior on small clinical corpora.

**Xu et al. (2025)** assembled the largest genuinely clinical dataset in this corpus: psychiatrist–patient dialogues from 1,160 outpatients at the Shanghai Mental Health Center, comprising roughly 15,000 minutes of transcribed Mandarin audio with corresponding electronic medical records covering 25 diagnoses. Ground truth derives from psychiatrist EMR documentation rather than self-report, and the extraction pipeline was validated against a purpose-built test set of 50 EMR cases manually reviewed by specialist psychiatrists. Methodologically this study is the most complete in the section: 138 validated clinical features and 177 assessment scale items, an ensemble classifier over LLM outputs, LIWC counts, TF-IDF weights and OpenSMILE prosodic features, SMOTE oversampling for minority classes, 10-fold cross-validation, Mann–Whitney U tests with FDR correction for feature ranking, and McNemar's test comparing supervised fine-tuned against zero-shot extraction. Its limitations are environmental rather than procedural — real-world clinical noise degraded the acoustic features, and Mandarin-centric training restricts transfer.

**Xin et al. (2024)** used the IMPACT-ME qualitative dataset, comprising 102 end-of-treatment interviews from 34 sets of depressed adolescents, parents, and therapists, nested within a randomised controlled trial. Two design decisions distinguish it. First, fine-tuning was deliberately declined in favour of frozen embeddings with weighted classifiers, on the grounds that positive instances were too sparse to train on — an explicit acknowledgment that method must follow data size. Second, cross-validation was grouped by subject ID to prevent leakage across the adolescent–parent–therapist triplets, making this the **only study in the section with documented subject-level leakage control**. Label sparsity was severe enough that some categories could not be trained at all, having fewer than four positive instances.

---

## 2.2 Social media and platform corpora

Three studies construct corpora from public platform text. The critical variable across them is not platform but label provenance.

**Qi et al. (2025)** introduced two Chinese datasets — SOS-HL-1K (1,249 posts, suicide risk) and SocialCD-3K (3,407 posts, multi-label cognitive distortion) — crawled from the "Zoufan" blog on Weibo and cleaned and anonymised by removing usernames and URLs. This study has the strongest annotation protocol in the section: three annotators with clinical psychology backgrounds performed double-blind annotation, with disagreements resolved through discussion with a senior licensed psychologist of more than five years' experience, and agreement quantified by **both Fleiss' κ and Krippendorff's α**. The experimental protocol is correspondingly careful — supervised baselines trained across five random seeds, LLMs evaluated over five runs at five temperature settings (0.1 to 0.9), with paired-samples *t*-tests at α = 0.05. Its headline finding, that traditional supervised models still outperform LLMs on complex clinical classification, carries more weight because of that protocol.

**Nanda et al. (2024)** used the Self-reported Mental Health Diagnoses (SMHD) corpus, where labels derive from users' own diagnostic disclosures on Reddit rather than from clinical assessment or expert annotation. The construction pipeline is a sequence of heuristics: regex-based linguistic cleaning and token pruning, condition keyword lists built from DSM-5 headings and extended with synonyms, misspellings, vernacular terms and abbreviations, cosine-similarity filtering of posts against clinical terms at a threshold of 0.5, and random downsampling of the control group to approximately 8,000 posts. A medical expert supplied the domain keywords. Each step is defensible individually, but together they determine which users enter the corpus, and the study is candid that evaluation rests on a single English-language dataset with no clinical validation.

**Sood et al. (2024)** created SMILE-College, 793 records of student narrative feedback filtered and annotated from the College Pulse Student Voice Survey. Annotation followed a two-stage human-machine collaborative process — preliminary annotation by one graduate student, validation by another, disagreements resolved collaboratively — and the authors identify the emergence of a "Mixed" sentiment category as a substantive finding rather than a labelling inconvenience. No formal agreement statistic is reported for the two-stage process. The dataset is small and the study concedes that decoder-based LLMs produced inconsistent output formatting that complicated post-processing.

**Table 2.1 — Label provenance across the corpus-building studies**

| Provenance tier | Mechanism | Studies | Agreement statistic reported |
|---|---|---|---|
| Expert clinical annotation | Psychiatrist/psychologist coding of clinical or platform text | Xu et al. (2025); Qi et al. (2025); Roy et al. (2025) | Fleiss' κ + Krippendorff's α (Qi); Cohen's κ 0.74/0.72 (Roy); psychiatrist-reviewed test set (Xu) |
| Structured self-report instrument | PHQ-8 / BDI-II administered under protocol | Ohse et al. (2024); Sood et al. (2023); Bucur et al. (2024) | Not applicable |
| Trained non-clinical annotators | Graduate students, bilingual validators, relevance raters | Sood et al. (2024); Bucur et al. (2024) | Majority-vote and unanimity gold standards (Bucur); none reported (Sood) |
| Platform self-disclosure | User-stated diagnosis matched by keyword patterns | Nanda et al. (2024) | None |
| Model-generated pseudo-label | LLM assigns training labels at scale | Aggarwal et al. (2024); Hu et al. (2025) | None (Aggarwal); human proofreading (Hu) |

---

## 2.3 Synthetic and simulated corpora

Two studies generate rather than collect data, and both report fidelity problems that make them more valuable as cautionary evidence than as demonstrations.

**De Duro et al. (2025)** produced CounseLLMe, 400 simulated counselling dialogues of 20 quips each — 200 English (Claude-3 Haiku with GPT-3.5 Turbo, roles reversed) and 200 Italian (Haiku with LLaMAntino) — with a professional psychotherapist providing clinical feedback during prompt development. Evaluation is unusual and worth noting for §4: rather than surface similarity metrics, the study reconstructs dialogues as Textual Forma Mentis Networks and profiles emotion using Plutchik lexicons, comparing against 24 human counselling transcripts from the HOPE dataset with Kruskal–Wallis tests on network distances and z-scores against a random null model. Manual coding after data collection checked for role-swapping and hallucination behaviours, and found both: Italian-language generation suffered role-swapping hallucinations and dialogue interference, and the models failed to reproduce the anger and frustration characteristic of human patients.

**Bucur et al. (2024)** tested synthetic augmentation directly, generating 30 synthetic Reddit-style posts for each of 90 BDI-II responses (2,700 per model) using GPT-3.5 and Llama-3 8B, then evaluating whether these improved semantic retrieval of depression symptoms from the eRisk 2023 corpus of roughly four million sentences. Relevance was established by top-*k* pooling (*k* = 50) with three human annotators producing majority-voting and unanimity gold standards, evaluated by Average Precision, R-Precision, P@10 and NDCG@1000. The result is negative and clearly characterised: the generated queries were too specific and introduced non-helpful detail that degraded retrieval relative to the original questionnaire responses. A secondary finding is equally useful — MPNet, fine-tuned for semantic search, outperformed MentalRoBERTa, fine-tuned on mental health text, inverting the intuitive expectation that domain pre-training dominates.

---

## 2.4 Annotation protocols and label provenance

Three studies treat the production of labels, rather than the collection of text, as the object of investigation.

**Roy et al. (2025)** built a diagnostic annotation layer over the PRIMATE dataset, prompting models to identify the specific sentences and text spans in social media posts that evidence PHQ-9 and GAD-7 criteria, with outputs constrained to clean JSON or Python lists to prevent extraction failure. Ground truth was constructed in two stages: GPT-4o generated candidate annotations, and three anonymised expert clinicians from an Indian non-profit institution validated a subset, achieving Cohen's κ of 0.74 for PHQ-9 and 0.72 for GAD-7. The resulting datasets were released. The study is candid that fine-tuning proved difficult, with the base MentalLLaMA model failing zero-shot tasks by repeating its input verbatim.

**Aggarwal et al. (2024)** is the section's most direct interrogation of label provenance, comparing four annotation sources on identical Reddit data — SMHD dictionary matching against Llama3, MentaLLaMA, and Samantha-Mistral — and then fine-tuning downstream classifiers on each. Two findings matter methodologically. First, the LLM annotators exhibited severe severity inflation, with the large majority of posts labelled Severe and one model producing no Mild labels at all. Second, classifiers trained on LLM pseudo-labels showed large train–validation gaps (95.8% against 70.31% for Llama3), which the authors read as overfitting to unreliable labels. Taken together this constitutes empirical evidence that LLM-generated training labels are not a neutral substitute for expert annotation.

**Hu et al. (2025)** constructed a large Chinese psychological training corpus — 155k single-turn QA pairs, 11k multi-turn dialogues, and 10k textbook knowledge QA items extracted via LLM agents — using a three-step pipeline of generation, **evidence judgment**, and refinement. The evidence-judgment stage is the notable component: KimiChat extracts matching text segments from the source context for each generated sentence, providing a grounding check against unsupported generation. A safety-check prompt was applied during dialogue refinement. Human proofreaders validated the generated multi-turn and knowledge-based pairs. The authors identify the residual risk plainly, noting potential generation bias from using LLMs to compile supervised fine-tuning data — the same concern that Aggarwal et al. demonstrate empirically.

---

## 2.5 Methodological appraisal of the data foundations

Four observations follow from reading these twelve studies together.

**Clinical data is the exception.** Only four of twelve studies use data generated in a clinical or semi-clinical encounter, and only one — Xu et al. — exceeds a thousand participants. The remainder rely on platform text, questionnaire instruments, or generated dialogue. Since Sections 3 through 6 largely evaluate methods developed on these corpora, claims about clinical performance in this literature rest on a narrow empirical base.

**Agreement statistics are rarely reported.** Of the twelve studies, three report a formal inter-annotator agreement statistic: Qi et al. (Fleiss' κ and Krippendorff's α), Roy et al. (Cohen's κ, 0.74 and 0.72), and Bucur et al. (majority-vote and unanimity gold standards from three annotators). The remaining nine either use single annotators, use unquantified multi-stage validation, or derive labels from self-report or model output. Where a corpus becomes a shared benchmark, unquantified annotation quality propagates silently into every study that subsequently uses it.

**Class imbalance is endemic and unevenly handled.** It is named as a limiting factor by Sood et al. (2023), Xin et al., Xu et al., and Aggarwal et al. Handling ranges from explicit — SMOTE oversampling and 10-fold cross-validation in Xu et al., weighted loss functions and subject-grouped folds in Xin et al. — to absent. Sood et al. (2023) report the consequence directly: transformer fine-tuning lost to TF-IDF baselines under weighted F1 on an imbalanced clinical corpus.

**Leakage control is almost entirely undocumented.** Only Xin et al. explicitly group cross-validation folds by subject to prevent the same participant appearing in both training and test partitions. Given that several corpora here contain multiple documents per participant — interviews with adolescents, parents and therapists; multiple posts per Reddit user — this is a material gap, and one that inflates reported performance in ways no metric will reveal.

**Table 2.2 — Corpus scale and validation characteristics**

| Study | Corpus | Scale | Ground truth source | Imbalance handling | Leakage control |
|---|---|---|---|---|---|
| Ohse et al. (2024) | KID (+ DAIC/E-DAIC) | Semi-clinical interviews | PHQ-8 self-report | Not reported | Not reported |
| Sood et al. (2023) | I-DAIC | 626 documents | PHQ-8 self-report | Acknowledged, unresolved | Not reported |
| Xu et al. (2025) | SMHC dialogues | 1,160 outpatients, ~15,000 min | Psychiatrist EMR + 50-case expert test set | SMOTE + 10-fold CV | Not reported |
| Xin et al. (2024) | IMPACT-ME | 34 subjects, 102 interviews | Qualitative content coding | Weighted loss | **Subject-grouped 4-fold CV** |
| Qi et al. (2025) | SOS-HL-1K; SocialCD-3K | 1,249 + 3,407 posts | 3 clinical annotators + adjudicator | Not reported | Not reported |
| Nanda et al. (2024) | SMHD subset | ~8k control posts | Platform self-disclosure | Downsampling | Not reported |
| Sood et al. (2024) | SMILE-College | 793 records | 2-stage student annotation | Not reported | Random 75/5/20 split |
| De Duro et al. (2025) | CounseLLMe | 400 dialogues | Synthetic (HOPE as reference) | Not applicable | Not applicable |
| Bucur et al. (2024) | eRisk 2023 + synthetic | ~4M sentences; 2,700 synthetic/model | 3 annotators, majority + unanimity | Not applicable | Not applicable |
| Roy et al. (2025) | PRIMATE + released sets | Randomised subsets | GPT-4o proposal + 3 clinician validation | Not reported | Not reported |
| Aggarwal et al. (2024) | Reddit (r/mentalhealth, r/depression) | 5,000 posts | LLM pseudo-labels (4 sources compared) | 5-fold CV | Not reported |
| Hu et al. (2025) | Proposed Chinese corpus | 155k + 11k + 10k items | LLM generation + evidence judgment + proofreading | Not reported | Not reported |

**A concluding observation on synthetic data.** Both studies that generated training or query data report fidelity failures — over-specific synthetic queries that degraded retrieval (Bucur et al.), and role-swapping hallucinations in non-English simulation (De Duro et al.) — and the study that used model-generated labels at scale documented systematic severity inflation (Aggarwal et al.). Against this, Hu et al. demonstrate that an explicit evidence-judgment stage can impose grounding discipline on generated data. The methodological implication carried forward into §3.2 and §6.1 is that synthetic data in this domain requires a verification stage as a matter of course, not as an enhancement.

---

*Papers in this section:* Ohse et al. 2024 (P01); Sood et al. 2023 (P54); Xu et al. 2025 (P36); Xin et al. 2024 (P32); Qi et al. 2025 (P04); Nanda et al. 2024 (P52); Sood et al. 2024 (P64); De Duro et al. 2025 (P05); Bucur et al. 2024 (P50); Roy et al. 2025 (P14); Aggarwal et al. 2024 (P55); Hu et al. 2025 (P60).


---

# 3. Model Adaptation Paradigms

## 3.0 Purpose and placement

Section 2 established that clinical mental health data is scarce, small, imbalanced, and frequently annotated without documented agreement. This section examines what researchers do about it. Fourteen of the sixty-six studies (21.2%) — the largest single grouping in this review — have as their primary contribution a technique for adapting a general-purpose language model to a mental health task rather than a corpus, a benchmark, or a clinical evaluation.

Four adaptation strategies are represented, and they are best understood as occupying different positions on a single trade-off between the cost of changing model weights and the cost of controlling model behaviour at inference time. Prompt engineering changes nothing and controls at inference (§3.1). Fine-tuning changes weights and accepts the compute and data cost (§3.2). Retrieval augmentation leaves weights untouched but constrains generation against an external evidence store (§3.3). Orchestration frameworks compose several models or tools without adapting any of them (§3.4). A fifth, smaller line abandons generation entirely and treats the model as a feature extractor (§3.5).

The section closes (§3.6) with what is, in this reviewer's assessment, the most consequential finding in the chapter: adaptation studies are systematically weaker at evaluating their own output than any other group in the corpus.

---

## 3.1 Prompt engineering and structured reasoning

Three studies treat the prompt as the object of investigation, holding model weights fixed.

**Patil et al. (2026)** conducted the cleanest ablation of reasoning strategies in the corpus, comparing Chain-of-Thought, Self-Consistency CoT, Few-Shot CoT, and Tree-of-Thought on a single reasoning-oriented model (o3-mini) across five Reddit benchmarks — Dreaddit, CSSRS, SDCNL, DepSeverity, and RedSam. Holding the model constant while varying only the reasoning scaffold isolates the contribution of the prompting strategy in a way that multi-model comparisons cannot. The metric suite is unusually complete for this literature, extending beyond accuracy and F1 to Matthews Correlation Coefficient, Quadratic Weighted Kappa, Mean Absolute Error, and both ROC and PR AUC — appropriate choices for the imbalanced, ordinal tasks involved. The findings are differentiated rather than uniform: Few-Shot CoT performed best on multi-class tasks (CSSRS, DepSeverity), plain CoT and SC-CoT on binary tasks (Dreaddit, SDCNL), and Tree-of-Thought was inconsistent throughout. Two limitations bear on interpretation. No inferential statistics are performed — strategies are compared descriptively across datasets, so no claim of significant difference is licensed. And the authors report that performance degrades in multi-class and long-text settings and remains highly sensitive to minor phrasing variation, which is itself a finding about the fragility of prompt-based adaptation.

**Kim et al. (2025)** developed LLM4CBT, a prompt-alignment framework with a three-part architecture — therapist persona, CBT technique concepts and examples, and preferred clinical behaviours — explicitly positioned as training-free to avoid the cost of parameter updates. Evaluation is conducted on both real and synthetic data: real therapist utterances from a merged HighQuality and HOPE corpus (366 dialogues, 7,669 therapist utterances) with outputs compared against ground-truth human therapist act labels across 13 act types and 5 categories, and simulated multi-round conversations against LLM-generated patient profiles where "estimated" automatic thoughts elicited in conversation are checked against ground-truth automatic thoughts embedded in the profile. Testing model pacing against deliberately reluctant "passive" patients is a thoughtful stress condition. The study is candid about the circularity risk in its own design: the evaluation pipeline depends on automated LLM-based classifiers and annotators, so the instrument measuring CBT alignment shares the failure modes of the system being measured. Real-data evaluation was also restricted to single rounds to conserve context window.

**Xu et al. (2024)** — Mental-LLM — spans this subsection and the next, and is placed here because its prompt taxonomy is the most systematic in the corpus. The zero-shot template decomposes into four components (TextData, PromptPart1-S, PromptPart2-Q, OutputConstraint), with three enhancement strategies compared against a basic condition: context enhancement, mental health enhancement (instructing the model to act as a psychologist), and their combination. Few-shot and chain-of-thought variants extend the design. The study then crosses this prompting axis with instruction fine-tuning, making it the only study in the section to quantify the prompting-versus-tuning trade-off directly on identical tasks. Its finding that compact fine-tuned models (Mental-Alpaca 7B, Mental-FLAN-T5 11B) match task-specific Mental-RoBERTa and exceed GPT-4 in zero- and few-shot settings is the strongest evidence in this review that prompt-based adaptation of large proprietary models is not the efficient frontier for classification tasks.

---

## 3.2 Supervised and parameter-efficient fine-tuning

Five studies update model weights. Read together, their most striking common feature is the compute range they span — from eight A100 GPUs to a single consumer card to 4-bit quantised edge deployment — which functions as an implicit statement about who can participate in this research.

**Lai et al. (2023)** built Psy-LLM through a two-stage supervised pipeline: domain pre-training on 2.85 GB of crawled Chinese psychology data over 100,000 iterations, followed by downstream fine-tuning on 56,000 PsyQA question–answer pairs validated by Tsinghua University. Training ran on a single V100 (32 GB). The evaluation protocol is dual and, for 2023, comparatively rigorous: intrinsic metrics (perplexity, ROUGE-L, Distinct-1, Distinct-2) alongside human evaluation in which six psychology-faculty students scored 200 model-generated and ground-truth pairs on helpfulness, fluency, relevance, and logic. Two expert psychologists checked the cleaned crawl. The authors concede that outputs fall short of human quality and that the unidirectional autoregressive architecture constrains contextual memory.

**Maurya et al. (2025)** compared four lightweight sequence-to-sequence models — T5-small (60M), FLAN-T5-small (80M), BART-base (139M), GODEL-base (220M) — fine-tuned on 20,500 QA pairs compiled from four public counselling resources, with a 70/30 split and training on a single T4. The methodological interest lies in reporting hardware metrics (parameter count, memory footprint, inference latency) alongside quality metrics, making deployability an explicit evaluation axis rather than an aspiration. The quality metrics themselves are the weakness: ROUGE-1/2/L, BLEU-4, and perplexity are *n*-gram overlap measures, poor proxies for empathy or clinical appropriateness, and the human assessment was conducted by a **single non-expert evaluator** — the thinnest human evaluation in the entire corpus. The authors also acknowledge that the training data received no professional curation.

**George et al. (2024)** fine-tuned Mistral-7B Instruct v0.1 with QLoRA on the counsel-chat dataset, running on a single RTX 3090 (24 GB). Evaluation departs from *n*-gram metrics in favour of PsychoBench, assessing Emotional Intelligence Scale and Empathy Scale scores against human reference averages drawn from prior literature, with F-tests and *t*-tests for significance. Applying psychometric instruments designed for humans to a model is of contested construct validity, but it is a more defensible proxy for counselling quality than BLEU, and the parametric testing is more than most studies in this subsection attempt.

**Gumilang et al. (2024)** pursued cultural rather than architectural adaptation, developing an Indonesian student mental health chatbot through a three-stage pipeline: global pre-training on Counsel Chat, expert-guided retraining on 1,800 locally sourced Indonesian entries, and L2 regularisation to counter overfitting on the small local corpus. Psychological experts guided the dataset enrichment. Evaluation combines training and validation accuracy tracking with User Acceptance Testing among 58 students on Likert-scaled ease of use, responsiveness, and satisfaction. The methodological limitation is that accuracy curves and satisfaction ratings jointly say little about clinical quality, and the authors note the system has no crisis detection or intervention protocol.

**Bookanakere et al. (2024)** fine-tuned GPT-2 (1.5B) quantised to 4 bits, with a documented configuration (group_size 128, damp_percent 0.01, desc_act False) chosen to fit strict resource constraints. The pipeline transforms tabular psychiatric lifestyle data into narrative paragraphs before training, evaluated on a held-out partition of 1,000 cases. Two limitations are conceded and both are material: quantisation entails precision loss, and the source dataset is synthetic, so tabular-to-text transformation may not resemble clinical language at all.

**Table 3.1 — Compute footprint and evaluation instrument across fine-tuning studies**

| Study | Base model | Method | Hardware | Primary evaluation | Human evaluation |
|---|---|---|---|---|---|
| Lai et al. (2023) | PanGu 350M / WenZhong 110M | Domain pre-training + SFT | V100 32GB | Perplexity, ROUGE-L, Distinct-1/2 | 6 psychology students, 200 pairs, 4 dimensions |
| Xu et al. (2024) | Alpaca 7B / FLAN-T5 11B | Multi-task instruction FT | 8 × A100 80GB | Balanced accuracy, cross-dataset transfer | Not reported |
| George et al. (2024) | Mistral-7B Instruct | QLoRA | 1 × RTX 3090 24GB | PsychoBench EIS/Empathy, F-test, *t*-test | Human norms from literature |
| Maurya et al. (2025) | T5/FLAN-T5/BART/GODEL (60–220M) | SFT | 1 × T4 16GB | ROUGE, BLEU-4, perplexity + hardware metrics | **1 non-expert evaluator** |
| Gumilang et al. (2024) | GPT-4-based | SFT + L2 regularisation | Not reported | Train/validation accuracy | 58 students (UAT, Likert) |
| Bookanakere et al. (2024) | GPT-2 1.5B | 4-bit quantised FT | Edge-constrained | Accuracy, precision, recall, F1 | Not reported |

---

## 3.3 Retrieval-augmented and knowledge-grounded architectures

Three studies leave weights untouched and constrain generation against external evidence. All three invoke hallucination reduction as motivation; they differ sharply in whether they substantiate it.

**Kharitonova et al. (2025)** built a RAG system over the Clinical Practice Guidelines of the Spanish National Health System covering adult depression and paediatric ADHD, using semantic search on paragraph embeddings (text-embedding-ada-002) with a strict negative-constraint prompt confining answers to retrieved content. The architecture deliberately isolates the model's reasoning ability from its parametric topic knowledge. Evaluation used 20 expert-authored questions across the two guidelines, rated by a specialist clinician on three structured Likert scales with independent verification by a second medical expert. The **Veracity scale is the notable instrument**: scored from −1 to +1 and explicitly penalising non-answers, it prevents a system from scoring well simply by refusing to respond — a failure mode that abstention-based designs invite. The authors state that hallucination was eliminated by the closed-database design; that is an architectural argument rather than a measurement, and should be read as such. Notably, the open-source LLaMA models answered more often and more accurately than GPT-3, which declined 25% of ADHD questions.

**Guo et al. (2024)** integrated GraphRAG over a knowledge graph constructed from DSM-5 and ICD-11 criteria with EmoLLM for symptom extraction, requiring no additional training. Consultation dialogues are segmented into *k*-round groups (*k* = 6), candidate symptoms extracted, then **validated and deduplicated against the knowledge graph** before a CoT-based diagnostic step. That validation stage is the most concrete hallucination-control mechanism in the section: rather than trusting retrieval to suppress fabrication implicitly, it re-checks each extracted symptom against a structured clinical ontology. The evaluation is appropriately ablated — zero-shot model comparison, backbone substitution within the framework, segmentation-length variation, and ablation studies — though it rests on a single small dataset (MMDA, 524 samples).

**Bhanu Sree et al. (2024)** combined RAG with LangChain agents executing specialised tools (CSV, PDF, PubMed) in parallel, routing queries by source type. The evaluation is almost entirely operational: time to first token (P50, P95), tokens per second, latency per minute, with qualitative comparative feedback on conciseness, contextual accuracy, helpfulness, and relevance. High latency outliers up to 495 seconds are reported. **No hallucination measurement is performed**, despite grounding in PubMed being the system's stated rationale, and the study relies on general pre-trained models without domain-specific updates.

---

## 3.4 Orchestration and hybrid pipelines

Two studies compose components without adapting any of them, and both illustrate an evaluation problem worth naming explicitly.

**Kamoji et al. (2024)** built a two-stage pipeline in which an ensemble classifier — selected from SVM, logistic regression, Random Forest, Bagging, AdaBoost — predicts mental health status from a 41,000-entry survey dataset with 25 features, after which Google Gemini generates personalised natural-language insight from that prediction. The architecture is defensible and arguably prudent: the diagnostic decision stays with an interpretable classical model, and the LLM handles only explanation. Feature selection via scikit-learn scores was used to refine the user-facing questionnaire. Two problems limit what can be concluded. Reported accuracy near 99% on self-report survey data is, as the authors themselves concede, suggestive of overfitting to synthetic or highly correlated fields. And **the LLM component is never evaluated** — no assessment of insight quality, factual accuracy, or safety appears, despite the generated reports being intended for psychiatrist review.

**Singh et al. (2024)** documented MindGuide, a LangChain composition using LLMChain with ConversationBufferMemory over GPT-4 at temperature 0.5, delivered through a Streamlit interface. The architectural documentation is clear and reproducible. The evaluation consists of a qualitative walkthrough of four conversation stages. There are no metrics, no dataset, no comparison condition, and no formal human evaluation — the authors state this plainly as a limitation. This matters beyond the individual paper because the system is explicitly positioned as an early identification assistant for **anxiety, depression, and suicidal thoughts**, with no crisis escalation protocol, guardrail, or safety evaluation reported. It is included in this review as evidence about the state of the field's publication standards, and it is revisited in §6.3 and §7.4.

---

## 3.5 Embedding-based adaptation

**Luna-Jimenez et al. (2024)** represents a distinct strategy: abandoning generation and using the LLM as a frozen feature extractor. Last-layer 4,096-dimensional hidden-state d-vectors were extracted from Llama-2-7b-chat and MentaLLaMA-chat-7B (loaded in 4-bit NF4 via bitsandbytes), averaged temporally, ranked by F-ANOVA filter, and passed to conventional downstream classifiers (SVM, logistic regression, k-NN, Nearest Centroid, decision trees, random forests, MLPs) tuned on a development split. Evaluation used 80/10/10 splits on Counsel-Chat and 7Cups with weighted F1 reported alongside **95% confidence intervals** — one of the few studies in this section to quantify uncertainty in its headline metric. The substantive finding is that roughly 75% of embedding dimensions are redundant for this task, permitting large reductions in downstream cost. The stated limitation is important for anyone reusing the method: selected dimensions show low overlap across datasets, so the feature-selection ranking is dataset-specific rather than a transferable property of the representation.

---

## 3.6 Methodological appraisal of the adaptation literature

**Evaluation quality is inversely related to engineering ambition.** This is the section's central finding. The studies that build the most — full pipelines, agentic orchestration, deployed interfaces — evaluate the least. Singh et al. report no metrics at all; Kamoji et al. never evaluate the generative component of a two-stage system; Bhanu Sree et al. measure latency but not accuracy or hallucination. Conversely the narrowest studies evaluate best: Patil et al. report ten metrics across five datasets, Luna-Jimenez et al. report confidence intervals, Kharitonova et al. designed a scoring scale specifically to close an abstention loophole. A reader of this literature should treat architectural novelty and evidential strength as largely independent.

**Generation quality is measured with instruments known to be inadequate.** Four studies generating therapeutic text rely wholly or partly on ROUGE, BLEU, or perplexity. These measure *n*-gram overlap with a reference and are insensitive to empathy, clinical appropriateness, or harm. The alternatives visible in this section — PsychoBench scales (George et al.), act-label distribution matching against human therapists (Kim et al.), expert Likert rating with a non-answer penalty (Kharitonova et al.) — are all better aligned to the construct, and none has been adopted widely.

**Human evaluation, where present, is thin.** Across fourteen studies, human evaluation ranges from six psychology students rating 200 pairs (Lai et al.) and 58 students in acceptance testing (Gumilang et al.), through a single expert clinician with a second-expert check (Kharitonova et al.), down to a single non-expert evaluator (Maurya et al.) and none at all (five studies). No study in this section reports inter-rater agreement for its human evaluation.

**Hallucination control is asserted architecturally more often than it is measured.** All three RAG studies invoke hallucination reduction; one implements an explicit verification stage (Guo et al.'s knowledge-graph symptom validation), one argues from closed-database design without measuring (Kharitonova et al.), and one measures nothing (Bhanu Sree et al.). This continues the pattern identified in §2.5, where generated data required a verification step to be trustworthy, and it sets up the distinction drawn in §6.1 between hallucination *mitigation* and hallucination *evaluation*.

**Compute access shapes the method distribution.** The hardware range — eight A100s (Xu et al.) to one T4 (Maurya et al.) to 4-bit edge deployment (Bookanakere et al.) — is not incidental. Three studies frame parameter-efficient or quantised adaptation explicitly as enabling deployment in low-resource settings, which is precisely where clinician shortages are most acute. The methodological consequence is that the most deployable systems are trained on the smallest and least curated corpora, compounding the data-quality concerns of §2.

**Table 3.2 — Evaluation adequacy across the adaptation studies**

| Adaptation strategy | Studies | Quantitative task metrics | Generation-quality instrument | Human evaluation | Hallucination measured |
|---|---|---|---|---|---|
| Prompting | Patil, Kim, Xu | All three | Act-label match (Kim) | LLM-based (Kim) | No |
| Fine-tuning | Lai, Maurya, George, Gumilang, Bookanakere | All five | ROUGE/BLEU (Lai, Maurya); PsychoBench (George) | 4 of 5, quality varies | No |
| RAG | Kharitonova, Guo, Bhanu Sree | Guo only | Expert Likert (Kharitonova) | Kharitonova (2 experts); Bhanu Sree (informal) | Verification stage (Guo) |
| Orchestration | Kamoji, Singh | Kamoji (classifier only) | None | None | No |
| Embeddings | Luna-Jimenez | Yes, with 95% CIs | Not applicable | No | Not applicable |

---

*Papers in this section:* Patil et al. 2026 (P28); Kim et al. 2025 (P38); Xu et al. 2024 (P30); Maurya et al. 2025 (P35); Gumilang et al. 2024 (P53); George et al. 2024 (P57); Bookanakere et al. 2024 (P63); Lai et al. 2023 (P17); Kharitonova et al. 2025 (P27); Guo et al. 2024 (P51); Bhanu Sree et al. 2024 (P61); Kamoji et al. 2024 (P59); Singh et al. 2024 (P62); Luna-Jimenez et al. 2024 (P58).


---

# 4. Benchmark Construction and Automated Evaluation

## 4.0 Purpose and placement

Section 3 closed on a diagnosis: the studies that build the most evaluate the least, and generation quality in that literature is routinely assessed with instruments — ROUGE, BLEU, perplexity — insensitive to the constructs that matter clinically. This section examines the response. Six of the sixty-six studies (9.1%) have as their primary contribution an evaluation artefact: a benchmark, a scoring protocol, or a framework for deciding when automated evaluation can be trusted at all.

The section is placed before human and clinical evaluation (§5) deliberately. The recurring question in §5 is whether expert raters are necessary — an expensive commitment that constrains sample size throughout that literature. That question is only answerable once the automated alternative has been characterised, including its documented failure points. Two of the six studies here address the question directly by evaluating LLM judges against human experts on identical material.

Three groupings emerge, distinguished by where ground truth comes from. Examination-grounded benchmarks inherit it from professional licensing instruments (§4.1). Expert-anchored benchmarks generate it from panels of practising clinicians (§4.2). Judge-reliability studies treat the relationship between the two as the object of measurement (§4.3).

The section's overall finding, stated at the outset because it inverts §3, is that **methodological rigour in this corpus is concentrated here**: five of six studies report inferential statistics, three report formal reliability coefficients, and two explicitly quantify uncertainty in their headline estimates.

---

## 4.1 Examination-grounded competency benchmarks

Three studies derive ground truth from standardised professional examinations, inheriting decades of psychometric development at no cost.

**Nguyen et al. (2025)** constructed CounselingBench from professional licensing standards: 1,612 unique multiple-choice questions across 138 clinical case studies, each containing demographics, presenting problems, and mental status examination detail, with expert-written rationales. The evaluation design is the largest model sweep in the corpus — 22 models crossed with five core competencies (Intake, Assessment & Diagnosis, Treatment Planning, Counseling Skills, Ethics) under zero-shot, few-shot, chain-of-thought, and self-consistency decoding. Its critical design decision is pairing each medical-specialised model (BioMedGPT, Asclepius, Meditron, MentaLlama, Clinical-Camel, Med42, OpenBioLLM) with its *own* general-purpose counterpart, which isolates the effect of domain fine-tuning from architecture. The finding that medical models systematically underperform their generalist bases by 4.2 percentage points is therefore attributable rather than merely correlational, and the authors trace the mechanism through manual annotation of reasoning errors on 100 responses by three expert annotators, identifying context-interpretation trade-offs — biomedical tuning introducing reading errors. Competency mapping was performed by two psychiatrists with a licensed mental health counsellor as tiebreaker. Statistical support is appropriate: paired *t*-tests for accuracy differences, chi-square for reasoning-error distributions. Beyond accuracy, ROSCOE reasoning metrics, BERTScore, ROUGE-1/L and cosine similarity assess reasoning quality. The conceded limitations are format and provenance: multiple-choice cannot capture empathy or therapeutic alliance, and a US licensing exam carries limited applicability to the Global South.

**Xu et al. (2025)** built the first integrated Chinese benchmark, combining the Chinese Counselor Qualification Exam (744 single-choice and 200 multiple-choice items, 2023–2024) with translated social media diagnostic screening on Dreaddit (1,151 posts) and SDCNL (1,517 posts). The two-task structure is the methodological contribution: it separates *theoretical knowledge* from *applied diagnostic performance*, and finds these dissociate — models strong on examination content are not correspondingly strong on classification. Fifteen models spanning 1.5B to 671B parameters and both dense and mixture-of-experts architectures were queried through a programmatic API harness at default parameters with no temperature adjustment, a choice that maximises reproducibility at the cost of not exploring decoding sensitivity. Class balance was maintained in SDCNL test sets, and the authors document a specific failure pattern: models over-predict the "anxiety" class under uncertainty. Analysis is descriptive only — accuracy percentages compared across parameter scales and release timelines, with no inferential testing. Ground truth quality is uneven across the three sources, professional examiners for the CAS exam but Amazon Mechanical Turk workers for the two social media corpora.

**Hanss et al. (2025)** took 150 single-answer multiple-choice questions from the Psychiatry Test Preparation and Review Manual and administered each ten times to GPT-3.5, GPT-4, and GPT-4o, allowing up to fifteen attempts to obtain ten valid single-letter responses. The repetition is the point. Rather than reporting a single accuracy figure, the study computes **response consistency via frequency variance** across trials and tests it as a predictor of correctness, alongside separately elicited pre-answer self-reported confidence (1–100). The result — consistency predicts accuracy while self-reported confidence does not — supplies a deployable proxy for reliability that requires no ground truth at inference time, which is precisely what a clinical deployment would need. Statistical treatment is the most careful in this subsection: chi-square tests with Bonferroni correction at α = .01, *t*-tests for consistency, and point-biserial correlations for predictors. Decoding parameters are documented (temperature 0.6, top_p 0.7). The authors flag two threats candidly: the MCQ format cannot assess interactive dialogue, and the questions may already sit in model training data — a contamination risk intrinsic to benchmarks built from published materials.

**Table 4.1 — Examination-grounded benchmark parameters**

| Study | Instrument | Scale | Models | Repetition | Inferential statistics |
|---|---|---|---|---|---|
| Nguyen et al. (2025) | Professional licensing standards | 1,612 MCQs, 138 case studies | 22 (13 medical + matched generalists) | 4 prompting/decoding conditions | Paired *t*-tests; chi-square |
| Xu et al. (2025) | Chinese Counselor Qualification Exam + 2 social corpora | 944 exam items; 2,668 posts | 15 (1.5B–671B) | Single pass, default parameters | None (descriptive) |
| Hanss et al. (2025) | Psychiatry Test Preparation and Review Manual | 150 MCQs × 10 trials | 3 (GPT family) | **10 trials per item** | Chi-square (Bonferroni, α=.01); *t*-tests; point-biserial *r* |

---

## 4.2 Expert-anchored benchmarks

Two studies generate ground truth from clinicians rather than inheriting it from an instrument, and both convert that expense into evaluative depth unavailable to multiple-choice designs.

**Li et al. (2026)** assembled the largest clinical expert panel in the corpus. COUNSELBENCH-EVAL comprises 100 real patient questions from CounselChat, with four responses each — three LLM-generated and one from a verified human therapist — rated **blind** by 100 licensed or professionally trained practitioners across the United States (LPCs, LCSWs, LMFTs, psychologists, psychiatrists), all individually verified. Rating covers six dimensions with deliberately heterogeneous scales matched to the construct: 5-point Likert for Overall, Empathy, Specificity and Toxicity; 4-point for Factual Consistency; binary for Medical Advice. Raters extracted supporting text evidence and wrote rationales, so judgements are traceable to specific spans rather than being holistic impressions. Inter-rater reliability is reported as Krippendorff's α — appropriate for the mixed scale types involved — and inference uses Wilcoxon signed-rank tests for pairwise comparison with Kruskal-Wallis and chi-square examining whether rater experience or time-on-task influenced ratings, a form of rater-effect control almost absent elsewhere in this corpus.

The study's second component is adversarial. Ten clinicians authored 120 questions targeting six failure modes empirically identified in the first phase, and five *different* practitioners evaluated 1,080 resulting responses — a separation of question-authors from response-evaluators that prevents self-marking. Hallucination is operationalised as Factual Consistency scoring with extraction of incorrect sentences validated against expert annotation; safety as Medical Advice flags capturing unauthorised clinical or medication recommendations, plus Toxicity flags for harmful or dismissive language. The study also evaluates LLM-as-Judge setups against its own expert ratings, reporting accuracy and F1. A pilot excluded MentalLLaMA-Chat-13B, MentalLLaMA-33B-Lora and Meditron-70B for high invalid-response rates — a documented exclusion that is itself a finding about domain-tuned models. Limitations are single-turn interaction and reliance on scarce publicly available non-deidentified data.

**McBain et al. (2025)** repurposed the Suicide Intervention Response Inventory (SIRI-2) — 24 hypothetical patient remarks paired with two clinician responses each, 48 items total — as an LLM benchmark. The design decision that gives the study its force is prompting deliberately *without* engineering: original SIRI-2 instructions only, zero-shot, to isolate baseline competency rather than optimised performance. Because SIRI-2 carries published norms, model scores are positioned directly on a human scale spanning expert suicidologists, clinical PhDs, master's-level counsellors, and untrained K-12 school staff. Reporting the resulting placements — ChatGPT-4o comparable to master's counsellors, Claude 3.5 Sonnet above post-trained professionals, Gemini 1.5 Pro comparable to K-12 staff — is far more interpretable than an accuracy percentage. Three independent research accounts prompted each model, supporting test-retest correlation. Statistical treatment accounts for the nested item structure through linear regression, with z-score outlier detection at |z| > 1.96, conducted in Stata 17.1 under STROBE reporting. Whether models fabricated rationales was checked and recorded in an appendix, though not formally scored. The stated limitation is precise: the study measures *evaluative* competency — the model as referee — not active engagement with a person in crisis.

---

## 4.3 Judge reliability and the limits of automated evaluation

**Badawi et al. (2026)** addresses the question the rest of this section raises: when can an LLM judge substitute for a human expert? The scale is substantial — MentalBench-100k comprising 10,000 conversations drawn from MentalChat16K, EmoCare and CounselChat, and MentalAlign-70k comprising 70,000 ratings. From 1,000 curated contexts, ten responses each were generated (one human, nine models) and rated by four LLM judges and three human experts with graduate-level or licensed psychiatric backgrounds, across seven attributes organised into a **Cognitive Support Score** (guidance, informativeness, relevance, safety) and an **Affective Resonance Score** (empathy, helpfulness, understanding).

The statistical apparatus is the most developed in the corpus. Agreement is decomposed into consistency ICC(C,1) and absolute agreement ICC(A,1) — a distinction that matters because a judge can rank responses correctly while being systematically miscalibrated, and only the second coefficient detects it. Systematic bias is reported directly as the LLM–human difference. Precision is quantified through 95% bootstrap confidence interval widths from 1,000 nonparametric iterations, with two-way mixed-effects ANOVA variance decomposition and paired *t*-tests supporting inference across 28 judge-attribute combinations. Ratings were aggregated to model level to filter conversation-level noise. Human reference ratings and traditional error metrics (MSE, RMSE) serve as baselines.

The resulting Affective-Cognitive Agreement Framework does not deliver a blanket verdict on LLM judges but a conditional one, classifying where automated judgement is reliable and where human oversight remains mandatory. That conditional structure is the contribution: it converts an ideological dispute about automated evaluation into a calibration problem. Limitations are English-only, single-turn dialogue, the computational cost of running multiple large judges, and — notably — expert rater availability, three raters supporting 70,000 ratings.

---

## 4.4 Methodological appraisal of the benchmark literature

**Statistical rigour is markedly higher here than elsewhere in the corpus.** Five of six studies report inferential statistics, against roughly one in five across the adaptation literature of §3. Three report formal reliability coefficients (Krippendorff's α in Li et al.; ICC in Badawi et al.; test-retest correlation in McBain et al.), and two quantify uncertainty explicitly (bootstrap confidence intervals in Badawi et al.; Bonferroni-corrected thresholds in Hanss et al.). Xu et al. is the sole exception, reporting descriptive accuracy only despite the largest model sweep in the subsection.

**Stochasticity is being taken seriously, unevenly.** Hanss et al. administer ten trials per item and convert the variance into a reliability measure; McBain et al. use three independent instances for test-retest correlation; Li et al. fix decoding parameters and document them. Xu et al. run a single pass at default settings. Since identical prompts yield different answers across runs, single-pass benchmark results carry unreported variance, and the field has not yet converged on a repetition standard.

**The multiple-choice format is the binding constraint on §4.1.** All three examination-grounded studies concede that MCQ performance cannot capture empathy, therapeutic alliance, or interactive competence — the properties that matter most in the clinical settings these benchmarks are meant to inform. Expert-anchored designs (§4.2) recover open-ended assessment but at a cost visible in their sample sizes: 100 questions in Li et al., 48 items in McBain et al. The trade-off between construct validity and scale is unresolved in this literature.

**Contamination is acknowledged once and otherwise unaddressed.** Hanss et al. note that published examination questions may already appear in model training data. The same risk applies to every benchmark in §4.1 built from published instruments, and to any benchmark drawn from public forums. No study in this section reports a contamination check.

**Domain fine-tuning does not help, on two independent measurements.** Nguyen et al. find medical-specialised models underperform their matched generalist bases by 4.2 percentage points; Li et al. excluded three domain-tuned models from their pilot for high invalid-response rates. Combined with the §3 finding that compact instruction-tuned models beat far larger prompted ones on classification, the emerging picture is that *task*-directed adaptation succeeds where *domain*-directed adaptation does not.

**Table 4.2 — Evaluation rigour across the benchmark studies**

| Study | Ground truth source | Reliability statistic | Uncertainty quantified | Repetition | Rater-effect control |
|---|---|---|---|---|---|
| Nguyen et al. (2025) | Licensing exam key + 2 psychiatrists | Tiebreaker adjudication | No | Prompting conditions | Not reported |
| Xu et al. (2025) | Exam key + MTurk labels | None | No | Single pass | Not applicable |
| Hanss et al. (2025) | Published review manual key | Response consistency (variance) | Bonferroni α = .01 | **10 trials/item** | Not applicable |
| Li et al. (2026) | 100 licensed practitioners, blinded | **Krippendorff's α** | No | Fixed decoding | Kruskal-Wallis/chi-square on experience and time |
| McBain et al. (2025) | Expert suicidologist norms + historical cohorts | Test-retest correlation | z-score outlier detection | 3 instances | Nested-structure regression |
| Badawi et al. (2026) | 3 psychiatric experts, 70k ratings | **ICC(C,1) and ICC(A,1)** | **95% bootstrap CIs (1,000 iters)** | 4 judges × 7 attributes | Two-way mixed-effects ANOVA |

**A closing observation on self-scrutiny.** Two studies in this section — Li et al. and Badawi et al. — turn the field's evaluation apparatus on itself, testing whether LLM judges align with human experts on the same material. This is a methodological maturation worth naming: rather than adopting LLM-as-judge for convenience and defending it informally, both quantify the conditions under which it holds. The distinction Badawi et al. draw between consistency and absolute agreement is carried forward into §7.2, where it applies equally to the human rating protocols examined in §5.

---

*Papers in this section:* Nguyen et al. 2025 (P29); Xu et al. 2025 (P47); Hanss et al. 2025 (P49); Li et al. 2026 (P02); McBain et al. 2025 (P24); Badawi et al. 2026 (P46).


---

# 5. Human-Centred and Clinical Evaluation Designs

## 5.0 Purpose and placement

Section 4 characterised the automated alternative and established the conditions under which it holds — Badawi et al.'s separation of consistency from absolute agreement being the sharpest instrument the field has produced for that question. It also surfaced the constraint that governs this section: three human experts supporting seventy thousand ratings. Expert time is the scarcest resource in this literature, and almost every design decision examined below is shaped by it.

Fourteen of the sixty-six studies (21.2%) — tied with §3 as the largest grouping — place human judgement or human experience at the centre of evaluation. They are ordered here along a **validity ladder**. Vignette studies (§5.1) maximise experimental control at the cost of ecological realism. Expert-rater studies (§5.2) apply clinical judgement to real model outputs. Controlled trials and prospective deployments (§5.3) observe systems in use. Qualitative and ethnographic work (§5.4) studies naturalistic interaction without intervening. Population survey evidence (§5.5) describes what is actually happening at scale. Internal validity is highest at the top of this ladder; ecological validity is highest at the bottom, and no study achieves both.

Two findings frame the section. Inter-rater reliability reporting is substantially better here than anywhere else in the corpus. And the field's entire prospective evidence base consists of **one exploratory two-week trial that was not statistically powered**.

---

## 5.1 Vignette and standardised-case designs

Four studies present models with controlled clinical stimuli. All four multiply small vignette sets through repetition, which is how they achieve analysable sample sizes.

**Levkovich et al. (2025)** used six clinical vignettes from prior published research, administering each to four LLMs twenty times in parallel male and female versions — 480 base assessments, N = 960 evaluations in total. The comparison standard is exceptional: norms from 1,536 health professionals (518 general practitioners, 506 psychiatrists, 498 clinical psychologists) and 6,016 members of the public, inherited from the source studies. Scoring of open-ended diagnoses proceeded by automated string-search filters, with referral effectiveness and prognosis rated on 6-point scales. Statistical treatment used chi-square and Fisher's exact tests in SPSS 27 with Cramér's V effect sizes computed in R 4.4.1. The gender-balanced design doubles as a bias probe, comparing treatment decisions for consistency across parallel versions. The authors are direct about the ceiling on their claims: hypothetical vignettes, no multi-turn dynamics, no clinical validation, and black-box opacity preventing inspection of clinical rationale.

**Schnepper et al. (2025)** built the tightest experimental design in the section — a randomised 2 × 2 crossing gender with sexual orientation across 30 published eating-disorder vignettes, yielding 120 vignette variants evaluated in three separate rounds by each of two models, for 720 evaluations (360 observations per measure). The outcome instruments are validated psychometrics rather than ad-hoc scales: the RAND-36 Mental Composite Summary and the EDE-Q global score, which renders any bias effect interpretable in clinically familiar units. Analysis uses linear multilevel models with **crossed random effects** — a random intercept for vignettes capturing between-vignette variance and a nested intercept capturing within-vignette variance — with intraclass correlation coefficients testing replicability. Temperature was set to 0 to minimise stochasticity. Three limitations are conceded and matter: the source vignettes were heavily gender-imbalanced (only two originally male), the custom temperature controls are opaque and unverified, and MentaLLaMA produced data of such low quality that the general-versus-specialised comparison is substantially weakened.

**Thotapalli et al. (2025)** evaluated three GPT variants across 22 youth psychiatric emergency vignettes over four iterations (N = 264 responses), against two advanced practice nurse practitioners with a committee of three board-certified psychiatrists grading response quality. The reliability treatment is the strongest among the vignette studies: **quadratically weighted Cohen's κ** for clinician–LLM agreement, appropriate for ordinal triage categories where the distance between disagreements matters, alongside Fleiss's κ for inter-model consistency. The substantive finding is an error asymmetry — zero false negatives against up to four false positive admissions — which is the safety-preferable direction but carries resource implications. Vignettes were drafted using ChatGPT and refined by the research team, a circularity the study should be read against.

**Lauderdale et al. (2025)** ran three models across four standardised veteran vignettes over ten trials each (120 trials), scored against the Veterans Health Administration Risk Stratification Table and compared with 42 licensed mental health care providers. The instrument choice is the contribution: an operational structured professional judgement framework already in clinical use, rather than a research scale, with acute risk, chronic risk and treatment disposition rated separately. Separating acute from chronic risk is a distinction most studies in this corpus collapse. Analysis used independent-groups *t*-tests, one-way ANOVA with Tukey's HSD post hoc tests, and hierarchical regression in JASP. The authors concede that four vignettes cannot support counterbalancing of demographic factors, and note pointedly that existing VHA machine-learning risk models were validated largely on White male veterans.

**Table 5.1 — Vignette study designs**

| Study | Vignettes | Repetition | Total observations | Human comparator | Reliability statistic |
|---|---|---|---|---|---|
| Levkovich et al. (2025) | 6 (× male/female) | 20 per version | 960 | 1,536 professionals + 6,016 public (published norms) | Cramér's V effect sizes |
| Schnepper et al. (2025) | 30 → 120 variants (2×2) | 3 rounds | 720 | None (published literature source) | ICC for replicability |
| Thotapalli et al. (2025) | 22 | 4 iterations | 264 | 2 nurse practitioners + 3 psychiatrists | **Weighted Cohen's κ; Fleiss's κ** |
| Lauderdale et al. (2025) | 4 | 10 trials | 120 | 42 licensed providers | Not reported |

---

## 5.2 Expert-rater comparative studies

Three studies apply clinical judgement to real model outputs rather than controlled stimuli.

**Settanni et al. (2025)** evaluated 425 Italian-language Reddit posts (filtered from 4,462) across three models under two prompt conditions, producing 2,550 ratings against a gold standard from two licensed clinical psychologists. Models output only a numerical urgency score on an adapted Mental Health Triage Scale (1–7), customised for informal social media register. The evaluation is unusually complete, reporting continuous agreement (Pearson *r*) alongside binary classification metrics after dichotomising at the urgent threshold — accuracy, F1, precision, sensitivity, specificity, Cohen's κ and AUC — with repeated stratified 5-fold cross-validation over ten repetitions and temperature fixed at 0. Weighted Cohen's κ quantifies clinician inter-rater reliability. As in Thotapalli et al., the dominant error is over-triage, which the study characterises explicitly as the safety-relevant failure mode.

**Cui et al. (2025)** developed the Mind Guardian suicide intervention chatbot around a five-stage crisis protocol grounded in intervention manuals and the ACT model, deployed via a Gradio web platform with documented decoding parameters (temperature 0.5, top-p 0.8, max length 400, presence penalty 0.1). Twenty psychology professionals conducted guided therapy sessions with the system and completed an eight-statement questionnaire across six dimensions on 7-point Likert scales, including a dedicated Safety and Privacy dimension. Analysis is descriptive only — means, standard deviations, ranges — with no comparison condition and no inter-rater statistic, which limits the design to establishing expert acceptability rather than efficacy.

**Eberhardt et al. (2025)** is, by statistical standards, the most complete study in the entire corpus. Working from 1,131 video-recorded therapy sessions across 155 outpatients, it develops LLEAP — an automated rating scale measuring latent patient engagement — through a full psychometric construction pipeline: 120 candidate items pre-selected on distributional properties, exploratory factor loadings and item-total correlations, then validated against independent process and outcome scales. Reliability is reported as Cronbach's α = 0.952, McDonald's ω = 0.953, and average variance extracted = 0.715; model fit via multilevel confirmatory factor analysis gives CFI = 0.968, TLI = 0.956, SRMR = 0.022, and **RMSEA = 0.108** — the last exceeding conventional thresholds, and reported rather than suppressed. Overfitting is guarded against by 1,000-resample bootstrap optimism correction and 3-fold cross-validation. Transcription quality is quantified (WER 26.76%; BGE-M3 cosine similarity 0.90), a step almost no other study using transcribed speech takes. Llama 3.1 8B runs locally on secure institutional servers so patient data never leaves the institution, and code is published on OSF and GitHub. The trade-off is cost: roughly 60 hours of processing on an RTX 4090, and a patient-level sample of 155 that is modest for scale validation.

---

## 5.3 Controlled trials and prospective deployment

**Campellone et al. (2025)** provides the corpus's only randomised controlled trial. One hundred and sixty adults were randomised 1:1 to a generative AI arm (n = 81) or an identical rules-based comparator (n = 79) in a two-week double-blind decentralised trial. The methodological contribution is the safety architecture and its verification. Guardrails operate at four tiers: a proprietary classifier detecting potentially concerning language that blocks prompts and routes to helplines before any model call; an embedding-based off-topic classifier filtering instructions and gibberish; prompt-level clinical constraints; and output-level XML structure and banned-word checks. Readiness was tested pre-trial against 42 simulated patient personas, and — the most notable step — **all 2,207 generated text completions were manually annotated post-trial** by two coders with principal-investigator resolution, verifying guardrail success exhaustively rather than by sampling. Outcomes used validated instruments (CSQ-8 for satisfaction, WAI-SR Bond for working alliance) alongside engagement metrics. Analysis is descriptive only: the study was explicitly not powered for between-group inference, ran two weeks, and did not adjust for baseline severity.

**Patias et al. (2024)** describes the me_HeLi-D project, integrating GPT-4 into digital modules for adolescents aged 12–15 covering early screening from journal entries, CBT and mindfulness interventions, interactive lessons, and conversational chatbots. Planned evaluation is mixed-methods — pre/post surveys using the Mental Health Literacy Scale and Strengths and Difficulties Questionnaire, interaction logs, focus groups with adolescents, teachers and mental health professionals, and behavioural tracking. Data protection is specified concretely (AES-256 encryption, pseudonymisation, access controls, GDPR compliance). The study is ongoing and its conclusions rest on preliminary data, so it contributes a protocol rather than findings; it is included because it is the only prospective work with minors in the corpus, and because automated screening of adolescent journal entries raises consent questions the paper acknowledges but does not resolve.

---

## 5.4 Qualitative, ethnographic and naturalistic studies

Four studies observe interaction rather than staging it, and collectively they supply the corpus's only evidence about what these systems do outside a research protocol.

**Wang et al. (2025)** structured evaluation in three stages with deliberate separation of roles: co-design with five mental health professionals averaging fifteen years of experience, a field user study with 19 participants producing 95 transcripts, and transcript review by **four different** professionals who had not participated in the design. Reviewers used a think-aloud protocol over Zoom on randomised dialogue logs (24 per expert), analysed thematically with iterative consensus-building. Separating designers from evaluators prevents self-marking, a control absent from most system papers in §3. Thematic codes name specific clinical failure modes — toxic positivity, leading questions, insufficient Socratic depth — and PHQ-9 and GAD-7 scores contextualise participants.

**Song et al. (2025)** conducted semi-structured interviews with 21 participants recruited purposively and by snowball sampling from specialised online communities, with deliberate diversity across Indian, Nigerian, Brazilian and Central Asian participants. This is the corpus's most globally distributed sample, and the choice is methodologically motivated: general-purpose models carry embedded linguistic and cultural bias, so a Western-only sample would systematically miss cultural mismatch. The analysis formalises *therapeutic alignment* as a multidimensional construct for assessing whether human–AI interaction supports long-term psychological healing. Limitations are a small non-clinical sample, retrospective self-report, and no clinical outcome measurement.

**Iftikhar et al. (2025)** ran an 18-month ethnography (May 2023 – October 2024) combining 110 self-counselling sessions conducted by seven trained peer counsellors — who met in 60 weekly focus groups to evaluate LLM behaviour — with 27 simulated multi-turn sessions independently and blindly reviewed by three licensed clinical psychologists. The longitudinal design is unique in the corpus. Inductive coding refined 41 initial codes to 15 ethical risks across five themes, each mapped to formal professional standards (APA, ACA, NASW), following Braun and Clarke's thematic analysis. Mapping to codified professional ethics rather than to author intuition is what gives the resulting framework normative force. No quantitative analysis is reported, and the study covers only prompted rather than fine-tuned models, on a single CBT-focused platform, with all psychologists from one country.

**Moore et al. (2026)** analysed real chat logs from 19 users reporting psychological harm — 391,562 messages across 4,761 conversations. The pipeline is technically careful: transcripts de-identified with Microsoft Presidio and Faker; tree-structured chat histories arising from message regeneration linearised into ancestral chains; 28 codes across five categories applied by gemini-3-flash-preview with **confidence thresholds raised for high-risk codes** (≥ 9 versus ≥ 7) to maximise precision where errors are most costly. Validation is layered: a random 560-message sample annotated by seven co-authors including a board-certified psychiatrist, plus **full manual verification of every suicidality and violence code** by two co-authors. Agreement is reported as Cohen's κ for LLM–human and Fleiss' κ for inter-annotator, with accuracy, precision, recall and F1. Conversational dynamics are modelled through per-message regressions on log-transformed remaining conversation length with participant-clustered standard errors, participant-normalised means with 95% confidence intervals, and transition log-lift calculations. The study is candid that agreement is moderate and prone to false positives on subjective codes, the sample is small and self-selected, and no objective clinical outcomes exist.

---

## 5.5 Population survey evidence

**Stade et al. (2026)** surveyed 1,871 US adults between August and October 2024 using stratified sampling across age, sex and race/ethnicity to approximate national demographics, with hypotheses preregistered at aspredicted.org. All respondents answered demographic, psychopathology and treatment-use items; self-identified users additionally answered questions on how, why and for what they use LLMs, plus perceptions of usefulness, therapeutic alliance, and the importance of memory. The headline estimate — 24% of respondents using LLMs for mental health, extrapolating conservatively to 14–18 million US adults — is the only population-scale figure in the corpus, and the linkage to treatment access barriers (cost 79%, insurance 61%, provider availability 54%) grounds the entire literature in a demand context that model-evaluation studies cannot supply. Group comparisons are reported with p-values. Limitations are inherent to the design: cross-sectional self-report supports no causal inference, coverage is single-country and single-window, and screening measures substitute for diagnoses. **This study's extraction is OCR-derived** — the source PDF carries no text layer — and should be verified against the original before citation.

---

## 5.6 Methodological appraisal of the human evaluation literature

**Reliability reporting is stronger here than anywhere else in the corpus.** Six of fourteen studies report a formal agreement or reliability coefficient: quadratically weighted Cohen's κ and Fleiss's κ (Thotapalli et al.), weighted Cohen's κ (Settanni et al.), Cohen's and Fleiss' κ (Moore et al.), ICC (Schnepper et al.), α/ω/AVE with full CFA fit indices (Eberhardt et al.), and Cramér's V effect sizes (Levkovich et al.). Set against three of twelve in §2 and none in §3, this is the clearest evidence that measurement discipline in this field tracks proximity to clinical practice.

**Expert availability sets sample size, not the research question.** The pattern is consistent: two clinicians establishing a gold standard for 2,550 ratings (Settanni et al.), three psychologists reviewing 27 sessions (Iftikhar et al.), four reviewers for 95 transcripts (Wang et al.), twenty experts for a single questionnaire (Cui et al.). Vignette studies work around this by inheriting published norms — Levkovich et al. borrowing 1,536 professionals they never recruited — which is efficient but ties findings to whatever the source studies measured.

**Repetition is standard here, unlike in §4.** All four vignette studies administer multiple trials (20, 3, 4, and 10 respectively), and two fix temperature at 0 for determinism. The stochasticity problem that §4.4 identified as unresolved in benchmarking is, in this subsection, routinely handled.

**The prospective evidence base is one underpowered trial.** Campellone et al. is the corpus's only RCT: two weeks, n = 160, explicitly not powered for between-group inference, run by the product developer, and excluding participants with recent suicidality — precisely the population whose safety is most at issue. Patias et al. is ongoing. No study in this corpus reports clinical outcomes from a powered trial of an LLM-based mental health intervention. Every efficacy claim in this literature rests on proxy measures.

**Conservative bias appears independently in two triage studies.** Thotapalli et al. report zero false negatives against up to four false positive admissions; Settanni et al. identify over-triage as the dominant error. Both find models err toward escalation. This is the safety-preferable direction, and it is worth contrasting with §6, where studies probing crisis handling find the opposite failure — models escalating too slowly, or not at all.

**Table 5.2 — Position on the validity ladder**

| Design | Studies | Internal validity | Ecological validity | Reliability statistic reported |
|---|---|---|---|---|
| Vignette / standardised case | Levkovich, Schnepper, Thotapalli, Lauderdale | High (controlled stimuli, repetition) | Low (hypothetical, single-turn) | 3 of 4 |
| Expert rating of real outputs | Settanni, Cui, Eberhardt | Moderate–high | Moderate | 2 of 3 |
| Controlled trial / deployment | Campellone, Patias | Moderate (randomised but underpowered) | High | 0 of 2 |
| Qualitative / naturalistic | Wang, Song, Iftikhar, Moore | Low (no control condition) | **Highest** (real use, real harm) | 1 of 4 |
| Population survey | Stade | Not applicable (descriptive) | High (national sample) | Not applicable |

**A closing observation.** The studies with the strongest ecological validity — Moore et al.'s real harm logs, Song et al.'s global interview sample, Iftikhar et al.'s 18-month ethnography — are precisely those that can make no causal claims, while the study with the most rigorous psychometrics (Eberhardt et al.) measures a single construct on a single sample. The field has not yet produced a design combining clinical realism with inferential power, and §7.4 returns to what such a design would require.

---

*Papers in this section:* Levkovich et al. 2025 (P10); Schnepper et al. 2025 (P19); Thotapalli et al. 2025 (P26); Lauderdale et al. 2025 (P31); Settanni et al. 2025 (P13); Cui et al. 2025 (P03); Eberhardt et al. 2025 (P42); Campellone et al. 2025 (P39); Patias et al. 2024 (P56); Wang et al. 2025 (P44); Song et al. 2025 (P45); Iftikhar et al. 2025 (P34); Moore et al. 2026 (P18); Stade et al. 2026 (P21).


---

# 6. Risk, Safety and Assurance Evaluation

## 6.0 Purpose and placement

This section is placed last among the substantive groupings because assurance evaluates everything preceding it. A corpus (§2) can encode bias; an adaptation method (§3) can introduce fabrication; a benchmark (§4) can miss the failure that matters; a clinical evaluation (§5) can be underpowered to detect harm. The ten studies grouped here — 15.2% of the corpus — treat those failures as the object of measurement rather than as limitations to be noted.

The section has a dual structure. Ten studies have risk evaluation as their **primary design**, and are treated individually in §6.1–§6.4. But risk fields are populated far more widely than that: hallucination methods appear in 37 of 66 studies, bias in 58, and safety in 61. Section §6.5 uses this corpus-wide extraction to make a claim the individual studies cannot support alone — that high nominal coverage conceals a much smaller body of actual measurement.

A note on §5's closing observation is warranted here. The triage studies found models erring toward *over*-escalation, which is the safety-preferable direction. The studies in this section, which probe crisis handling directly rather than incidentally, find the opposite.

---

## 6.1 Hallucination and factual grounding

Two studies operationalise hallucination as a measurable quantity, and they define it in incompatible ways — a divergence that is itself the subsection's finding.

**Linardon et al. (2025)** converts hallucination into a fully verifiable outcome: citation fabrication. Six literature reviews of roughly 2,000 words were generated in a 3 × 2 factorial design crossing disorder familiarity (major depressive disorder, binge eating disorder, body dysmorphic disorder) with prompt specificity (general, specialised). All 176 generated citations were manually extracted and exhaustively verified across Google Scholar, Scopus, PubMed and WorldCat, then classified as fabricated, real-with-errors, or accurate, with error subtypes recorded down to author, year, title, journal, volume, issue, page and DOI. DOI hallucination is disaggregated usefully into valid-but-irrelevant links versus wholly invalid identifiers. Analysis used two-tailed chi-square tests of independence with pairwise comparisons at *P* < 0.05.

The design's power comes from the factorial structure: 19.9% of citations were fabricated overall, but fabrication was concentrated in the less-visible disorders (28% and 29% for BED and BDD against 6% for MDD). Hallucination is therefore shown to be **conditional on informational terrain** rather than a fixed model property — a result no single-condition study could produce. The limitations are narrow scope: one model, one output per condition, and no test of whether retrieval augmentation or validation prompting would mitigate the effect.

**Kim et al. (2026)** defines a construct the factual literature does not capture. *Affective hallucination* denotes emotionally immersive responses evoking false social presence — a model simulating emotional capacity it does not possess. Prompts were sourced from five mental-health subreddits (ADHD, PTSD, OCD, Asperger's, Depression) to produce AHaBench (500 prompts) and AHaPairs (5,000 preference pairs). Assessment uses a 7-point rubric across three dimensions: Emotional Enmeshment, Illusion of Presence, and Fostering Overdependence. Crucially, the automated judge is **validated against clinical ground truth** — two independent licensed psychiatrists rated outputs, with human–GPT-4o agreement at *r* = 0.85 against inter-human agreement of *r* = 0.95, plus MAE of 0.35 and cross-judge agreement, with means and standard deviations across three random seeds.

The study also supplies mitigation rather than only diagnosis, comparing DPO alignment against SFT, SFT+DPO and few-shot baselines across model sizes from 7B to 72B, and verifying on MMLU, GSM8K and ARC that alignment does not degrade general reasoning. Testing for capability regression after a safety intervention is rare in this corpus and should be standard. Limitations are Reddit-sourced data with acknowledged demographic skew (young, Western, male), single-turn evaluation, and potential author annotation bias.

---

## 6.2 Bias and stigma auditing

Two studies treat differential treatment as the measurand.

**Yeo et al. (2025)** built a closed-loop agent-to-agent design of unusual methodological care. A GPT-4 conversational agent interacted with GPT-3.5 Digital Standardised Patients across 97 demographic combinations of age, sex, race and income, each tested four to five times alongside controls, producing 449 transcripts and 4,502 agent responses. The critical control is **asymmetric information**: the DSPs remained agnostic to their own sociodemographic traits while the agent was informed of them through a separate input channel, so any linguistic difference must originate with the agent rather than with differently-behaving simulated patients. Measurement used LIWC-22 across 13 primary and 30 exploratory markers, cross-validated with external Python NLP libraries, deliberately avoiding human raters to eliminate researcher subjectivity.

The statistical treatment is the most thorough of any bias study here: Shapiro-Wilk normality testing, *t*-tests and Mann-Whitney U for subgroup comparison, ANOVA and Kruskal-Wallis for multiple groups, univariate and multivariate linear regression, **Joinpoint regression** for piecewise trend analysis of tone across ten sequential dialogue bins, and group-based trajectory modelling. Analysing tone *trajectory* within conversations, not merely aggregate difference, captures bias that emerges over an interaction. Limitations are simulated rather than real patients, a single English-language model, and LIWC's insensitivity to subtler implicit bias.

**Moore et al. (2025)** examined stigma and clinical appropriateness together. A mapping review of ten clinical guideline documents (APA, VA, NICE) yielded 17 features of good therapy, used both to construct a "steel-man" system prompt — giving models their best chance rather than a strawman — and as the evaluation rubric. Experiment 1 applied modified US National Stigma Studies vignettes: 72 vignettes across four conditions with 14 questions, 1,008 questions total, measuring willingness to interact socially with the described character. Experiment 2 tested responses to ten acute stimuli including suicidal ideation and delusions, with and without transcript context of varying lengths.

Statistical rigour is high — bootstrapped 95% confidence intervals, *t*-tests with Bonferroni correction for stigma, z-tests of proportion with Bonferroni correction for appropriateness — and inter-rater reliability reaches **Fleiss' κ = 0.96**, the highest in the corpus. Sixteen human therapists supplied baseline responses, with classifier labels validated by a psychiatrist and computer scientist. The safety criterion is concrete: failing to challenge delusions, or supplying suicide-enabling information such as bridge lists, is classified as unsafe. Temperature was fixed at 0. Limitations include simplified multiple-choice stigma items and clipped transcripts that may generate non-sequiturs.

---

## 6.3 Crisis-safety and escalation testing

Three studies probe what happens when a user in crisis meets a deployed system.

**McBain et al. (2025)** conducted the largest safety audit by volume. Thirteen clinical experts (three psychiatrists, ten clinical psychologists) stratified 30 suicide-related questions into five risk levels using mean expert scores with explicit banding (very low 1–1.49 through very high 4.5–5). Each of three commercial chatbots was then queried **100 times per question, yielding 9,000 responses**, each independently coded by two researchers as direct or indirect with third-coder adjudication, and indirect responses further classified by referral type. Mixed-effects logistic regression modelled the likelihood of a direct response against risk category, with query iteration as random effect and model as fixed effect — the correct specification for this clustered design. The methodological contribution is stratifying refusal behaviour across five clinician-calibrated levels rather than a binary safe/unsafe split, which exposes inconsistency at intermediate risk that a binary framing would hide.

**Heston (2023)** is the smallest study here and produces one of the most consequential findings. All 25 conversational agents identified on a public repository were tested twice — once with general distress prompts, once with PHQ-9-anchored prompts — recording the severity point at which each agent referred to a human counsellor and the point at which it shut down. Anchoring escalation to PHQ-9 makes "too slow to escalate" quantifiable in clinically interpretable units rather than impressionistic. The distinctive move is continuing past shutdown to test restartability, revealing that **22 of 25 safety-triggered agents resume normal conversation once distress severity drops** — a loophole that a single-pass test cannot detect, and evidence that safety shutdowns are not durable states. The study also concludes that general-purpose guardrails, not agent-specific prompting, dictate shutdown points. Its limitations are real: a single evaluator (the author), fixed prompts, descriptive statistics only, and ChatGPT-3.5-era agents.

**Campbell et al. (2025)** conducted the corpus's only longitudinal safety study, collecting responses in Spring 2023 (5 prompts, 3 chatbots) and again in Summer 2024 (7 prompts, 7 chatbots). Two trained school counsellors with sixteen years' combined adolescent crisis experience coded responses for empathy level, presence of crisis resources, tone, lethality handling and urgency, with disagreements resolved by consensus; LIWC-22 supplied authenticity and emotional tone scores. Two design choices reflect genuine insight into the user population: only free accounts were used, reflecting adolescent access conditions, and prompts were framed as seeking help *for a friend*, capturing the proxy framing young people actually use — which also bypasses direct safety triggers. Verification extends to whether the correct hotline number was given (988 versus a malformed variant). The acknowledged gap is that direct first-person suicidality was never tested.

---

## 6.4 Adversarial and automated red-teaming frameworks

Three studies build reusable infrastructure for eliciting failure rather than measuring it once.

**Au Yeung et al. (2025)** introduced psychosis-bench, running 128 experiments (8 models × 16 scenarios) across 1,536 conversational turns. Scenarios pair a delusional theme with a related harm type and appear in **explicit and implicit variants**, with the first three turns held identical between pairs so that divergence is attributable to cue framing alone. Three orthogonal metrics are scored by an LLM judge: Delusion Confirmation Score (0–2, challenge/neutral/validate), Harm Enablement Score (0–2), and a binary Safety Intervention Score. Analysis used paired *t*-tests for the implicit-versus-explicit contrast and Spearman's rank-order correlation between harm enablement and delusion confirmation. Scenarios were clinician-written and validated, but **scoring was performed entirely by the LLM judge with no reported human validation** — a material weakness given that Kim et al. in §6.1 demonstrate such validation is achievable. Limitations are 16 scenarios and 12-turn conversations.

**Steenstra et al. (2026)** built the most elaborate framework in the corpus. Fifteen clinically validated personas — five empirically derived alcohol use disorder phenotypes crossed with three stages of change — were instantiated as patient agents with an embedded **dynamic cognitive-affective model**, managed by a simulation orchestrator with state persisted across checkpoints. A full factorial design crossed six therapist conditions with 30 stratified patient pairings across four longitudinal weekly sessions (180 dyads, 369 sessions completed). A four-stage repeated-measures cycle tracked pre-session outcomes, in-session crises and constructs, post-session alliance and fidelity, and between-session narratives. Metrics span therapeutic fidelity (MI adherence, complex reflection rate, reflection-to-question ratio) and safety (multi-class crisis detection covering ideation, threats to others, and severe decompensation). Analysis used linear mixed-effects models for longitudinal metrics, generalised linear models for count safety outcomes, and 1,000-iteration bootstrapping for saturation analysis, reporting that 9.68 pairings on average suffice to reach 95% metric saturation — a genuinely useful design parameter for anyone replicating this approach. Human validation covered clinical realism (9 psychology professionals) and dashboard usability (9 multidisciplinary stakeholders). Including a deliberately Harmful AI condition alongside commercial systems provides a lower anchor most evaluations lack.

**Cai et al. (2026)** developed PsyCrisis for reference-free safety evaluation in Chinese. A manually curated dataset of 608 real crisis utterances (289 suicide, 115 non-suicidal self-injury, 204 existential distress) was drawn from online discourse, with risk categories defined using WHO mhGAP and LIVE LIFE guidelines. Eight hundred open-ended responses were scored across five binary dimensions — empathy, emotion regulation advice, worry exploration, risk assessment, external referral — using psychologist-verbalised chain-of-thought reasoning, so each judgement is traceable to an expert-defined criterion rather than a holistic score. Reference-free design matters because curating gold answers for every possible crisis utterance is impractical. Validation is thorough: six clinical professionals annotated categories, scores and explanation preferences; agreement is reported as Cohen's κ = 0.697, F1 = 0.802 and Fleiss' κ; and judge rationales were compared by human pairwise preference across three judge setups. Annotator compensation is disclosed (20 RMB/hour) — the only study in the corpus to do so. Limitations are single-turn scope, Chinese-only context, and potential leniency bias in the LLM evaluator.

---

## 6.5 Corpus-wide appraisal: coverage without measurement

Restricting attention to the ten studies above would misrepresent the field. The extraction records risk methods across the whole corpus, and the aggregate picture is less reassuring than the coverage figures suggest.

**Table 6.1 — Risk evaluation across all 66 studies**

| Dimension | Studies with content | Share | Of which: actual measurement |
|---|---|---|---|
| Safety | 61 | 92% | **11** test output safety or crisis handling |
| Bias | 58 | 88% | **5** apply counterfactual, linguistic, or stigma-probe methods |
| Hallucination | 37 | 56% | **11** score or verify it |

**Safety coverage is dominated by data governance, not output testing.** Of 61 studies with safety content, 26 describe research-ethics or data-governance measures — IRB approval, consent, encryption, HIPAA or GDPR compliance, de-identification — and 24 discuss safety narratively. Only **11 actually test whether model output is safe**. Both categories are legitimate, but they answer different questions: encrypting a transcript protects a participant's privacy, and says nothing about whether the system will supply a bridge list to a person in crisis. Any synthesis reporting "92% of studies address safety" without this decomposition would materially mislead.

**Bias is overwhelmingly acknowledged rather than measured.** Of 58 studies with bias content, 13 explicitly note bias as a concern without evaluating it, and 40 offer descriptive or incidental treatment. Five apply a recognisable bias method: counterfactual manipulation (Schnepper et al., Levkovich et al.), linguistic instrumentation (Yeo et al.), and stigma-vignette probing (Moore et al., Nguyen et al.'s demographic case coverage). Given that the corpora characterised in §2 derive substantially from English-language Western platforms, and that Song et al. in §5.4 found cultural mismatch to be a leading user complaint, five measurement studies across 66 is a thin evidential base for any claim about fairness in this literature.

**Hallucination has the lowest coverage but the healthiest measurement ratio.** Of 37 studies, 11 measure or score it, 5 mitigate architecturally without measuring, and 21 discuss it only. The mitigation-without-measurement group is the one flagged in §3.6: retrieval augmentation is invoked as a hallucination control and then never tested. Kharitonova et al.'s claim that hallucination was eliminated by closed-database design is an architectural argument; Guo et al.'s knowledge-graph symptom validation is a verification stage; Bhanu Sree et al. measure nothing. Only the second constitutes evidence.

**The two hallucination constructs do not compose.** Linardon et al. measure factual fabrication; Kim et al. measure affective simulation. A system could score perfectly on the first while failing badly on the second — indeed a heavily-guardrailed system that never fabricates a citation may be precisely the one that over-performs emotional presence. The field currently lacks a framework integrating factuality, faithfulness (per Huang et al.'s taxonomy in §1.3) and affective hallucination into a single assurance account.

**Crisis findings contradict §5's triage findings, and the difference is methodological.** The triage studies of §5.1 found conservative over-escalation; the crisis studies here find under-escalation, non-durable shutdowns, and inconsistent guardrails at intermediate risk. The explanation lies in stimulus design. Triage studies present a complete case and ask for a rating; crisis studies present an escalating user in distress and observe behaviour. Single-turn rating tasks do not surface the failures that multi-turn escalation produces, which is a direct argument for the multi-turn designs of §6.4.

**Human validation of automated judges is inconsistent even within this section.** Kim et al. validate their GPT-4o judge against two licensed psychiatrists (*r* = 0.85 against an inter-human ceiling of 0.95); Cai et al. validate against six clinical professionals with κ = 0.697 and F1 = 0.802; Au Yeung et al. report no human validation of judge scoring at all. Since all three use LLM judges to produce safety verdicts, the difference matters: a judge's leniency bias — which Cai et al. name explicitly as a limitation — propagates directly into a safety conclusion.

**Table 6.2 — Design characteristics of the ten risk-primary studies**

| Study | Turn structure | Stimulus source | Judge | Human validation of judge | Inferential statistics |
|---|---|---|---|---|---|
| Linardon et al. (2025) | Single output | Generated reviews | Human (authors) | Not applicable | Chi-square, pairwise |
| Kim et al. (2026) | Single-turn | Reddit-sourced | GPT-4o | **2 licensed psychiatrists** | Pearson *r*, MAE, 3 seeds |
| Yeo et al. (2025) | Multi-turn simulated | Agent-to-agent, blinded DSPs | LIWC-22 (automated) | Not applicable | Joinpoint regression, GBTM, multivariate |
| Moore et al. (2025) | Single + context variants | Guideline-derived, stigma vignettes | gpt-4o classifier | Psychiatrist + CS validation; **Fleiss' κ = 0.96** | Bootstrap CIs, Bonferroni |
| McBain et al. (2025) | Single-turn ×100 | Expert-stratified queries | 2 human coders + adjudicator | Not applicable | Mixed-effects logistic regression |
| Heston (2023) | **Escalating multi-turn** | PHQ-9-anchored simulation | Single human (author) | Not applicable | Descriptive only |
| Campbell et al. (2025) | Single-turn, 2 phases | Proxy-framed prompts | 2 school counsellors | Consensus resolution | LIWC percentiles |
| Au Yeung et al. (2025) | **12-turn escalation** | Clinician-written scenarios | gpt-4o-mini | **None reported** | Paired *t*-tests, Spearman |
| Steenstra et al. (2026) | **4 longitudinal sessions** | 15 validated personas | Automated + orchestrator | 9 psychology professionals | LMM, GLM, bootstrap saturation |
| Cai et al. (2026) | Single-turn | 608 real crisis utterances | GPT-4o, expert CoT | **6 clinical professionals** | Correlations, κ, F1, majority vote |

---

*Papers in this section:* Linardon et al. 2025 (P25); Kim et al. 2026 (P43); Yeo et al. 2025 (P09); Moore et al. 2025 (P12); McBain et al. 2025 (P06); Heston 2023 (P65); Campbell et al. 2025 (P16); Au Yeung et al. 2025 (P11); Steenstra et al. 2026 (P23); Cai et al. 2026 (P48).


---

# 7. Cross-Cutting Methodological Quality

## 7.0 Purpose and placement

Sections 1 to 6 examined the corpus by contribution type. This closing section examines it by *quality*, and deliberately owns no papers: it reports across all 66 studies using the extraction fields directly. The purpose is to convert the preceding descriptive account into an evidence-based statement of what this literature can and cannot currently support, and thereby to establish the research gap this thesis addresses.

The appraisal is organised around four properties that determine whether a finding can be believed and built upon: whether claims are supported by inference (§7.1), whether measurement is reliable (§7.2), whether work can be reproduced (§7.3), and which designs are systematically absent (§7.4). Section §7.5 states the resulting gap.

One methodological caveat applies throughout. This appraisal rests on what studies *report*, extracted verbatim; it is not a validated risk-of-bias instrument such as MMAT or RoB 2, and §1.5 already conceded that limitation. Under-reporting and under-performance are therefore indistinguishable here. That said, in a literature where reproducibility depends on reporting, the distinction is less consequential than it might appear: an unreported method is, for practical purposes, an unavailable one.

---

## 7.1 Statistical rigour and inference

**Fewer than half the corpus supports its claims inferentially.**

**Table 7.1 — Statistical treatment across 66 studies**

| Treatment | Studies | Share |
|---|---|---|
| Inferential statistics reported | 28 | 42% |
| Descriptive statistics only | 31 | 47% |
| No statistical analysis reported | 7 | 11% |

The 31 descriptive-only studies are not uniformly at fault — the ten reviews and conceptual papers of §1 have no primary data to test, and several qualitative studies in §5.4 report thematic analysis appropriately. But the group also contains benchmark comparisons, model evaluations, and system studies where performance differences are asserted across conditions without any test of whether those differences exceed chance. Where a study reports that one prompting strategy or one model outperformed another and offers no inferential support, the ordering it establishes should be treated as provisional.

The distribution of tests indicates a field applying a narrow standard toolkit rather than matching method to design:

| Test family | Studies |
|---|---|
| *t*-tests | 10 |
| Regression (linear, logistic, hierarchical) | 6 |
| Chi-square | 5 |
| ANOVA | 4 |
| Bootstrap | 4 |
| Mixed-effects / multilevel models | 5 |
| Kruskal-Wallis | 3 |
| Explicit confidence intervals | 3 |
| Multiple-comparison correction (Bonferroni) | 2 |

Two absences are conspicuous. **Only two studies report multiple-comparison correction** despite many conducting dozens of comparisons across models, prompts, and metrics — Moore et al. and Hanss et al. being the exceptions. And **only three report explicit confidence intervals** on their headline estimates, so most reported differences carry unquantified uncertainty. Where studies repeatedly query the same model on the same items — a structure inherent to almost every benchmark and vignette design in this corpus — mixed-effects specifications are the appropriate response to the resulting clustering; five studies use them.

**Rigour is unevenly distributed across contribution types.**

**Table 7.2 — Methodological rigour by section**

| Section | n | Inferential statistics | Reliability coefficient | Code/data released |
|---|---|---|---|---|
| §1 Reviews & conceptual | 10 | 0 (0%) | 2 (20%) | 2 (20%) |
| §2 Data foundations | 12 | 4 (33%) | 2 (17%) | 4 (33%) |
| §3 Model adaptation | 14 | 3 (21%) | 0 (0%) | 5 (36%) |
| §4 Benchmarks | 6 | **5 (83%)** | **3 (50%)** | 1 (17%) |
| §5 Human & clinical evaluation | 14 | 6 (43%) | 5 (36%) | 2 (14%) |
| §6 Risk & assurance | 10 | **8 (80%)** | 2 (20%) | 1 (10%) |

The gradient confirms the section-level observations made throughout this chapter. Adaptation studies (§3) are the weakest on inference and report **no reliability coefficients at all**, while benchmark (§4) and risk (§6) studies are strongest. The inverse relationship between engineering ambition and evaluative rigour identified in §3.6 is visible here as a corpus-level pattern, not an artefact of which papers were read closely.

**The trajectory is improving, and steeply.**

**Table 7.3 — Rigour by publication year**

| Year | n | Inferential statistics | Reliability coefficient |
|---|---|---|---|
| 2023 | 4 | 0 (0%) | 0 (0%) |
| 2024 | 17 | 4 (24%) | 1 (6%) |
| 2025 | 36 | 16 (44%) | 9 (25%) |
| 2026 | 9 | 6 (67%) | 4 (44%) |

This is the most encouraging finding in the chapter. Inferential reporting rises from zero to 67% and reliability reporting from zero to 44% across four years. It also reframes the appraisal: much of the weakness documented above is concentrated in earlier work, and the field is professionalising rapidly. It further reinforces the §1.4 finding that prior reviews — whose search windows all close by August 2024 — characterise a methodologically weaker literature than the one now current.

---

## 7.2 Reliability and inter-rater agreement

**Fifty-nine of 66 studies involve human evaluation. Fourteen report any reliability coefficient.**

**Table 7.4 — Reliability statistics reported**

| Coefficient | Studies |
|---|---|
| Cohen's κ | 7 |
| Fleiss' κ | 5 |
| Krippendorff's α | 2 |
| ICC / intraclass | 2 |
| Cronbach's α, McDonald's ω, AVE | 1 |
| Test-retest correlation | 1 |
| **Any coefficient (unique studies)** | **14 / 66 (21%)** |

The consequential figure is the intersection: **45 of the 59 studies using human evaluation report no agreement statistic whatsoever.** Human judgement is the field's most trusted ground truth — 33 of 59 studies use licensed clinical professionals — yet in three quarters of cases the reader cannot know whether two raters would have agreed. Where a study reports that clinicians rated model responses favourably, without agreement data, that finding rests on an unquantified assumption of rater consistency.

Where agreement *is* reported, the range is instructive: Fleiss' κ = 0.96 (Moore et al.) at the top, against 0.613 inter-annotator and Cohen's κ = 0.566 for LLM–human agreement in Moore et al. (2026)'s harm-log coding, and κ = 0.697 in Cai et al. Coefficients in the 0.55–0.70 band are moderate, and the studies reporting them say so — the concern is the 45 studies where such a figure would likely be lower still and is simply absent.

Two methodological imports from §4 and §5 deserve wider adoption. Badawi et al.'s separation of **consistency ICC(C,1) from absolute agreement ICC(A,1)** distinguishes a rater who ranks correctly from one who is correctly calibrated — a distinction that applies to human panels as much as to LLM judges, and that no human-rater study in this corpus makes. And Eberhardt et al.'s full psychometric apparatus (α, ω, AVE, CFA fit indices, bootstrap optimism correction) demonstrates that classical test theory is applicable to LLM-derived measures; it is applied once.

---

## 7.3 Reproducibility and artefact availability

**Table 7.5 — Reproducibility markers across 66 studies**

| Marker | Studies | Share |
|---|---|---|
| Code, data, or models released | 15 | 23% |
| Hyperparameters specified | 14 | 21% |
| Hardware specified | 13 | 20% |
| Decoding parameters specified | 13 | 20% |
| Reporting standard followed (PRISMA, STROBE, CONSORT, MMAT, RoB 2) | 12 | 18% |
| Protocol preregistered | 2 | 3% |

Roughly one study in five documents the parameters required to reproduce it. **Decoding parameters are the most significant omission.** Temperature, top-p and sampling settings materially change model output; 53 of 66 studies do not report them. Since §4.4 established that repetition is inconsistently applied and §7.1 that confidence intervals are rare, a substantial share of reported performance differences in this corpus cannot be distinguished from sampling variance. The studies that do this well — Moore et al. and Settanni et al. and Schnepper et al. fixing temperature at 0 for determinism; Cui et al. and Li et al. and Heston reporting full decoding configurations — demonstrate that the cost of reporting is trivial.

Preregistration at 3% (Jin et al.; Stade et al.) is low even by the standards of adjacent fields, and is notable given that 28 studies conduct hypothesis tests. Kolding et al.'s finding, reported in §1.2, that models and prompts are so underspecified in this literature that replication is frequently impossible is independently corroborated by these figures.

---

## 7.4 Systematic design gaps

Four gaps recur across the corpus and are not attributable to individual studies.

**Single-turn evaluation dominates a multi-turn problem.** Of 56 empirical studies, 16 employ multi-turn, longitudinal, or repeated-measures designs; nine explicitly state single-turn scope, and most of the remainder are single-turn by construction. The consequence is demonstrated rather than hypothesised: §6.5 showed that triage studies presenting a complete case find conservative over-escalation, while crisis studies presenting an escalating user find under-escalation, non-durable shutdowns, and inconsistent guardrails. Heston's restartability finding — 22 of 25 agents resuming after a safety trigger once distress subsides — is undetectable in any single-pass design. Therapeutic relationships are longitudinal; the evaluation apparatus largely is not.

**The prospective evidence base is one underpowered trial.** Campellone et al. remains the corpus's only randomised controlled trial: two weeks, n = 160, explicitly not powered for between-group inference, conducted by the product developer, and excluding participants with recent suicidality. No study in this corpus reports clinical outcomes from an adequately powered trial. Every efficacy claim in this literature rests on proxy measures — benchmark accuracy, expert appropriateness ratings, satisfaction scores — none of which has been validated against patient outcomes.

**Linguistic and cultural coverage is narrow and unevenly examined.** Chinese-language work is well represented (10 studies), with smaller contributions in Italian, German, Spanish and Indonesian. But four studies explicitly note English-only scope as a limitation, the dominant corpora characterised in §2 are English-language Western platforms, and §6.5 established that only five studies apply any recognisable bias method. Song et al.'s globally distributed interview sample found cultural mismatch to be a leading user complaint — a finding the rest of the corpus is poorly equipped to investigate.

**Stochasticity is unaddressed in four studies out of five.** Twelve of 66 studies address repetition, repeated trials, or test-retest reliability. The remainder report single-pass results from systems that are non-deterministic by default. Hanss et al. demonstrated that repetition yields something valuable beyond error bars — response consistency across trials predicts accuracy while self-reported confidence does not, giving a deployable reliability proxy — yet the practice remains rare.

---

## 7.5 The gap addressed by this review

Six statements follow from the appraisal above, and together they define what this literature currently cannot support.

1. **No pooled effect estimate exists for any LLM mental health application.** All seven prior reviews synthesise descriptively (§1.4), and the heterogeneity of metrics, tasks, and ground-truth definitions documented across §2–§6 explains why.
2. **Human evaluation is the field's primary ground truth and is largely unvalidated.** Forty-five of 59 studies using human raters report no agreement statistic (§7.2).
3. **Safety coverage is nominally near-universal and substantively narrow.** Sixty-one studies address safety; 11 test whether model output is safe (§6.5).
4. **Bias is acknowledged far more often than measured.** Fifty-eight studies address bias; five apply a recognisable method (§6.5).
5. **Reproducibility is the weakest dimension.** One study in five reports decoding parameters, hyperparameters, or hardware; one in thirty preregisters (§7.3).
6. **Clinical efficacy is unestablished.** One underpowered exploratory trial constitutes the entire prospective evidence base (§7.4).

The present review addresses the first, second, third and fourth of these by extracting methodology — not results — uniformly across 66 studies with four dedicated risk fields, permitting the corpus-wide claims in §6.5 and §7.1–§7.3 that no prior synthesis could support. It cannot address the fifth or sixth, which require primary research rather than review.

What a stronger design in this field would require follows directly: multi-turn or longitudinal interaction rather than single-turn stimulus; repeated trials with reported decoding parameters and confidence intervals; human evaluation with reported agreement, ideally separating consistency from absolute calibration; safety evaluation that tests output behaviour rather than documenting data governance; bias evaluation using counterfactual manipulation with clinically interpretable outcome instruments; and, ultimately, powered trials measuring patient outcomes rather than proxies. Every one of these components already exists somewhere in this corpus — Steenstra et al.'s longitudinal simulation, Hanss et al.'s repetition protocol, Badawi et al.'s ICC decomposition, Heston's escalation anchoring, Schnepper et al.'s counterfactual psychometrics, Campellone et al.'s trial architecture. None exists in combination.

The trajectory documented in Table 7.3 suggests that combination is closer than the aggregate figures imply. Rigour is rising steeply year on year, and the 2026 cohort reports inferential statistics at 67% and reliability coefficients at 44% — roughly triple and seven times the 2024 rates respectively. The methodological weaknesses catalogued in this chapter are, to a substantial degree, characteristics of a literature's first three years rather than fixed properties of it.

---

*This section draws on all 66 studies in the corpus and owns no papers exclusively.*
