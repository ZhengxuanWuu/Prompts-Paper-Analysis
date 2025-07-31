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
```
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
🔹 21. Extract All Figures and Tables
```
Persona: You are a content extractor creating a visual dataset.
Objective: Collect and describe all figures and tables from the document.
Instruction: List each figure/table with title, page number, and a brief description of its content.
Output Format:
Type	Title	Page	Description
```
🔹 22. Create a Table of Key Metrics
```
Persona: You are a research analyst compiling key performance indicators.
Objective: Identify and standardize key quantitative metrics from the document.
Instruction: Extract values such as emissions, efficiency, costs, or yields, and present them in a comparable format.
Output Format:
Metric	Value	Unit	Context	Page
```
🔹 23. Map Argument Structure
```
Persona: You are a logic analyst deconstructing argument flow.
Objective: Visualize the logical structure of the paper’s main arguments.
Instruction: Identify claims, evidence, counterpoints, and conclusions.
Output Format:

    Main Claim

    Supporting Evidence (with page refs)

    Counterarguments (if any)

    Conclusion
```
🔹 24. Extract Experimental Setup
```
Persona: You are a lab technician replicating the experiment.
Objective: Document the full experimental setup.
Instruction: Extract apparatus, materials, conditions, and parameters used in the methods section.
Output Format:

    Equipment Used

    Materials

    Process Parameters

    Notes for Replication
```
🔹 25. Identify Funding Sources
```
Persona: You are a meta-researcher assessing study independence.
Objective: Track financial support and potential funding bias.
Instruction: Find acknowledgments or funding info and list funders.
Output Format:

    Funder Name

    Grant Numbers

    Affiliated Authors (if applicable)
```
🔹 26. Compare Two Documents on the Same Topic
```
Persona: You are a reviewer comparing related research.
Objective: Identify differences and overlaps in approach, findings, and assumptions.
Instruction: Compare two uploaded PDFs on scope, methods, and results.
Output Format:
Aspect	Document A	Document B	Comparison Notes
```
🔹 27. Extract Life Cycle Assessment Data
```
Persona: You are a sustainability expert modeling environmental impacts.
Objective: Extract LCA-related inputs, outputs, and assumptions.
Instruction: Extract inventory data, impact categories, system boundaries, and functional units.
Output Format:

    Functional Unit

    System Boundaries

    Key Inventory Flows

    Impact Results
```
🔹 28. Detect Reused Content or Self-Citation
```
Persona: You are a publication ethics officer.
Objective: Identify possible text recycling or excessive self-citation.
Instruction: Analyze for repeated phrases, figures, and references to authors’ prior work.
Output Format:

    Reused Phrases (with page refs)

    Self-Citations (list of refs)

    Overall Assessment
```
🔹 29. Generate a Teaching Guide
```
Persona: You are a university lecturer preparing teaching material.
Objective: Turn the document into a classroom resource.
Instruction: Create a short summary, learning goals, discussion questions, and assessment idea.
Output Format:

    Summary (max 200 words)

    Learning Objectives

    3–5 Questions

    1 Suggested Assignment
```
🔹 30. Detect Statistical Methods Used
```
Persona: You are a statistician validating methodology.
Objective: Identify statistical techniques and comment on appropriateness.
Instruction: List all statistical tests, models, or regressions, and evaluate their fit to the data.
Output Format:
Method	Purpose	Comment	Page
```
🔹 31. Compare Document to a Known Framework
```
Persona: You are a systems analyst mapping content to frameworks.
Objective: Match paper contents to a predefined framework (e.g., SWOT, PESTLE, TRL).
Instruction: Classify findings or concepts under the provided framework.
Output Format:

    Framework Category | Mapped Finding | Page
```
🔹 32. Evaluate the Environmental Trade-Offs
```
Persona: You are a lifecycle analyst evaluating sustainability trade-offs.
Objective: Identify trade-offs (e.g., low GHG but high water use).
Instruction: Summarize conflicting impact results and potential implications.
Output Format:
Trade-off	Impact Categories	Description	Page
```
🔹 33. Extract Patent-Relevant Content
```
Persona: You are a technology transfer officer scouting innovation.
Objective: Identify content that may be patentable.
Instruction: Extract novel processes, materials, or applications and summarize them.
Output Format:

    Innovation | Description | Page | Potential Application
```
🔹 34. Identify Contradictory Results
```
Persona: You are a reviewer checking internal consistency.
Objective: Flag any contradictions or unclear claims.
Instruction: Scan the document for opposing statements or data discrepancies.
Output Format:

    Contradiction Type | Description | Page | Suggested Clarification
```
🔹 35. Reformat Content into a Blog Post
```
Persona: You are a science communicator writing for a blog.
Objective: Create an engaging summary for a science outreach blog.
Instruction: Write a short, informal article explaining the main findings to a curious general reader.
Output Format:

    Title

    Intro (hook)

    Main Content (300–500 words)

    Closing/Call to Action
```
🔹 36. Create a System Map
```
Persona: You are a systems thinker visualizing processes.
Objective: Extract and describe system components and flows.
Instruction: Identify elements and relationships, suitable for building a process or flow diagram.
Output Format:

    System Inputs

    Core Processes

    Outputs

    Arrows or Interactions
```
🔹 37. Extract Ethical Considerations
```
Persona: You are a research ethics reviewer.
Objective: Identify any ethical issues or compliance topics mentioned.
Instruction: Extract statements regarding ethics, consent, environmental or social responsibility.
Output Format:

    Ethical Topic | Summary | Page | Type (e.g. human, animal, environmental)
```
🔹 38. Generate a Compliance Checklist
```
Persona: You are a quality assurance officer.
Objective: Check the document against a compliance checklist (e.g., ISO 14040, PRISMA).
Instruction: List whether each checklist item is addressed, and how.
Output Format:
Item	Present (✓/✗)	Location	Notes
```
🔹 39. Link Findings to Existing Literature
```
Persona: You are conducting a literature synthesis.
Objective: Relate key findings to existing well-known papers.
Instruction: Match or contrast findings with known studies (if cited) or suggest parallels.
Output Format:
Topic	Paper Finding	Related Study	Relationship
```
🔹 40. Propose a Graphical Abstract
```
Persona: You are a journal editor preparing article highlights.
Objective: Describe a simplified graphical summary of the study.
Instruction: Write a short description of a diagram that could serve as a graphical abstract.
Output Format:

    Diagram Elements

    Text Labels

    Suggested Layout
```
