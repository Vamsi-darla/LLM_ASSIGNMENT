Botswana IMF Report Analysis
This project analyses Botswana’s 2025 Article IV Consultation report using an AI-assisted PDF-to-dashboard pipeline in Google Colab.
Files
- vamsi_botswana_code.ipynb — notebook containing the pipeline and saved outputs.
- LICENSE — MIT License covering the project code.
How to Run
1. Open the notebook in Google Colab.
2. Download IMF Country Report No. 25/325: Botswana—2025 Article IV Consultation from the IMF website.
3. Rename the downloaded PDF to botswana.pdf and upload it to the Colab working directory.
4. Add your Gemini API key to Colab Secrets as New_key and enable notebook access.
5. Run all cells in order. Internet access and access to the configured Gemini model are required.
Pipeline
The notebook extracts and cleans PDF text, applies OCR, generates summaries, extracts financial indicators and thematic findings, builds a vector-based RAG index, compares single-query and multi-query retrieval, and produces a four-panel dashboard.
Outputs
Results are saved under botswana_project/results/, including JSON extractions, summaries, evaluation records, CSV tables and dashboard figures. Cached data are stored under botswana_project/cache/.
Evaluation and Limitations
Automated checks and LLM judge scores do not guarantee factual accuracy. Outputs require verification against the source PDF. Recorded limitations include an inflation-audit discrepancy, unanswered fiscal-reform retrieval and unresolved audit flags.
License
The project code is released under the MIT License. The IMF report remains subject to its own copyright and usage terms.
