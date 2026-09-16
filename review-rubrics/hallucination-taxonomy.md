Hallucination Taxonomy for Clinical AI

Purpose

This document classifies common hallucinations produced by medical large language models (LLMs) during clinical question answering.

⸻

Type 1 — Fabricated Medical Facts

Definition: The model invents clinical facts, laboratory values, diseases, or drug information that are not supported by evidence.

Example: Inventing a non-existent contraindication for aspirin.

Risk: Moderate to High

⸻

Type 2 — Unsupported Clinical Recommendation

Definition: The recommendation is medically plausible but lacks sufficient evidence or guideline support.

Example: Advising prolonged antibiotics without an indication.

Risk: Moderate

⸻

Type 3 — Diagnostic Hallucination

Definition: The model reaches an incorrect diagnosis despite the clinical presentation strongly supporting another condition.

Example: Diagnosing gastritis in a patient with classic STEMI symptoms.

Risk: Critical

⸻

Type 4 — Fabricated Guideline Citation

Definition: The model claims that NICE, WHO, AHA, or another guideline recommends something that the guideline does not actually state.

Example: “WHO recommends Drug X as first-line therapy” when no such recommendation exists.

Risk: High

⸻

Reviewer Checklist

Before approving any AI response, verify:

* Is every medical claim evidence-based?
* Are red flags identified?
* Is emergency escalation appropriate?
* Are drug doses and contraindications correct?
* Are guideline references genuine?

⸻

Severity Matrix

|Hallucination Type|Typical Severity|
|-------------------|---------------|
|Fabricated facts	         |Major|
|Unsupported recommendation	 |Minor–Major|
|Diagnostic hallucination	 |Critical|
|Fake guideline citation	 |Major|

Reviewer Note

A clinically fluent response is not automatically a safe response. Patient safety and evidence should always take priority over confident wording.