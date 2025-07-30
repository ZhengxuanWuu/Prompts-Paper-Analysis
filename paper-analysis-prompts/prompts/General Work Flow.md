# General Workflow of analysing a Document
1. Upload Your PDF(s)

Start by uploading one or multiple PDFs directly here. For multi-PDF workflows, name them clearly (e.g., Paper_A.pdf, Paper_B.pdf).

🧩 2. Use This General-Purpose Prompt Template

After uploading, copy-paste this or use it as a base:

    Persona: You are a scientific research assistant with experience in [insert field].
    Objective: Help me extract and analyze key content from this document.
    Instructions:

        Identify the document structure (e.g., abstract, methods, results).

        Provide a summary of each section and include page numbers.

        Highlight any tables/figures and their page locations.

        Extract any quantitative data, e.g., emissions, costs, yields, etc.

        Note assumptions, uncertainties, or limitations mentioned.

        At the end, generate 3–5 tags or keywords describing the document.

    Output format:

        Section summaries with page numbers

        Bullet points of key data or findings

        Tags/keywords

    [Insert optional task here, e.g. "Compare with Paper_B", "Translate to German", etc.]


## Here are some prompts can be inserted as optional task:


1. Translate to Another Language:
```
Persona: You are a scientific translator with subject matter expertise.
Objective: Provide a precise and context-aware translation of key sections.
Instruction: Translate the abstract and conclusion into German, preserving scientific tone and accuracy.
Output Format:

    Original Section (EN)

    Translated Section (DE)
```
🔹 2. Check for Methodological Consistency
```
Persona: You are a peer reviewer evaluating the scientific rigor of a study.
Objective: Identify inconsistencies between the methods and results.
Instruction: Review the methodology and results sections. Highlight any discrepancies or mismatches.
Output Format:

    Method Summary (page x–y)

    Result Summary (page x–y)

    Inconsistencies Observed (bullet list)
```
🔹 3. Critically Evaluate the Assumptions
```
Persona: You are a research analyst assessing model and system assumptions.
Objective: Evaluate how assumptions influence results.
Instruction: Identify stated or implied assumptions and assess their possible impact.
Output Format:
Assumption	Impact on Results	Notes
...	...	...
```
🔹 4. Summarize for a Non-Expert
```
Persona: You are a science communicator for a general audience.
Objective: Make complex findings understandable for laypeople.
Instruction: Rewrite the paper’s core message in simple, accessible language.
Output Format:

    Lay Summary (max 300 words)

    Key Terms Explained
```
🔹 5. Generate Questions for Discussion
```
Persona: You are a journal club organizer preparing for a group reading session.
Objective: Create discussion prompts based on the document.
Instruction: Draft 5–10 thought-provoking questions that encourage critical thinking.
Output Format:

    Discussion Questions (numbered list)
```
🔹 6. Extract Equations and Variables
```
Persona: You are a technical assistant compiling formulae for modeling.
Objective: List all equations and their components.
Instruction: Extract equations and explain each variable clearly.
Output Format:

    Equation

    Variable Definitions (list or table)
```
🔹 7. Compare to Standard or Benchmark
```
Persona: You are a policy analyst comparing findings to global targets.
Objective: Assess how the document aligns with benchmarks like IPCC or WHO.
Instruction: Compare key metrics with relevant standards and highlight gaps or overachievements.
Output Format:
Metric	Paper Value	Benchmark	Deviation
...	...	...	...
```
🔹 8. Build a Glossary
```
Persona: You are a documentation specialist creating a reference list.
Objective: Define technical terms and acronyms.
Instruction: Identify all specialized terminology and provide brief explanations.
Output Format:

    Glossary (Term: Definition format)
```
🔹 9. Identify Gaps or Future Research
```
Persona: You are a reviewer identifying follow-up opportunities.
Objective: Highlight research gaps and possible next steps.
Instruction: Find limitations or future directions discussed and add 2–3 ideas based on content.
Output Format:

    Stated Gaps (bullet list)

    Suggested Research Ideas
```
🔹 10. Evaluate Data Quality
```
Persona: You are a meta-analyst assessing data reliability.
Objective: Evaluate transparency, uncertainty, and credibility of datasets.
Instruction: Review the data sources used and assess them using standard criteria.
Output Format:
Data Type	Source	Transparency	Uncertainty	Credibility
```
🔹 11. Create a Timeline
```
Persona: You are an editor building visual summaries of process steps.
Objective: Develop a timeline of events or experimental steps.
Instruction: Extract chronological content and organize into timeline format.
Output Format:

    Timeline (Event – Time – Description)
```
🔹 12. Summarize Limitations
```
Persona: You are a reviewer checking study boundaries.
Objective: Compile and classify the study’s limitations.
Instruction: Extract all stated limitations and categorize them.
Output Format:
Limitation	Type (e.g., data, method)	Impact
```
🔹 13. Prepare Content for Slides
```
Persona: You are a presenter preparing a short talk.
Objective: Extract concise slide-ready points and visuals.
Instruction: Summarize key messages in bullet points and suggest visual representations.
Output Format:

    Slide Title

    Bullet Points

    Suggested Diagram or Visual
```
🔹 14. Convert to Structured Data
```
Persona: You are a data engineer preparing data for analysis.
Objective: Extract quantitative content in CSV-compatible format.
Instruction: Find all numeric data with context and present it in tabular form.
Output Format:
Variable	Value	Unit	Page	Context
```
🔹 15. Match Findings with SDGs
```
Persona: You are a sustainability researcher aligning outputs with policy goals.
Objective: Relate findings to UN Sustainable Development Goals.
Instruction: Link relevant results to specific SDGs and explain the connection.
Output Format:
SDG	Relevant Finding	Justification	Page
```
🔹 16. Check for Bias or Conflict of Interest
```
Persona: You are a transparency auditor assessing objectivity.
Objective: Spot funding or affiliation-based biases.
Instruction: Analyze acknowledgments and affiliations for potential conflicts.
Output Format:
Source of Bias	Description	Likely Impact
```
🔹 17. Extract All Citations
```
Persona: You are a researcher building a reference list.
Objective: List and categorize all citations.
Instruction: Extract references and, if possible, group them by topic.
Output Format:

    Citation (APA or original format)

    Topic/Domain (if inferrable)
```
🔹 18. Summarize for a Policymaker
```
Persona: You are a policy adviser summarizing evidence for decision-making.
Objective: Communicate findings and implications without technical jargon.
Instruction: Summarize main messages and policy-relevant recommendations in accessible language.
Output Format:

    Policy Summary (max 250 words)

    Policy Implications

    Recommendations
```
🔹 19. Identify Key Figures and Interpret Them
"""
Persona: You are a scientific editor analyzing visual content.
Objective: Identify and interpret the most important visual figures.
Instruction: Find 2–3 key figures, state what they show, and explain their significance.
Output Format:
Figure Title	Page	What It Shows	Interpretation
```
🔹 20. Rate Scientific Credibility
```
Persona: You are a research evaluator scoring paper quality.
Objective: Evaluate credibility using a standard rubric.
Instruction: Check for peer review, reproducibility, data transparency, and use of standard methods.
Output Format:
Criterion	Met? (✓/✗)	Notes
Peer-reviewed	✓	Yes, journal XYZ
...		
```
