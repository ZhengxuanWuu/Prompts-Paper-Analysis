# Prompts-Paper-Analysis
I categorise the prompts according to the potential purpose of reading/analysing a paper.
The purpose could be 
1. Extract information from a paper for literature review
2. Methodologies, how to solve a problem
3. Find datas, need to be specified
4. Find the research gaps from the paper
5. Discover trends in a scientific field, development and debate in methodologies
6. Compare your study with published paper, LCA results as example 

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

🔄 3. Compare Two PDFs

Once both PDFs are uploaded, you can ask:

    Compare the methods and results of Paper_A.pdf and Paper_B.pdf.
    For each, include:

        Page numbers

        Main methodological approach

        Key results or metrics

        Any limitations

Or:

    Extract the carbon footprint results from both papers and present them in a table, with units and assumptions if mentioned.

📌 4. Reference Text by Page Number

To explicitly ask for text on a page:

    Show me the text from page 12 of Paper_A.pdf, and summarize the main idea.

    OR

    What is discussed in pages 5–7? Are there tables or figures?

📊 5. Extract Tables or Create Structured Overviews

Use:

    Extract all tables from this document. Present them in markdown or a simplified format.

    OR

    Extract any LCA inventory data (inputs, outputs, units) if present and present as a structured table.

🏷️ 6. Auto-tag or Classify the Document

    Based on the content, generate 5–10 keywords or research tags that would help categorize this paper in a library.
    Include research domain, methodology, key metrics, and topic focus.
