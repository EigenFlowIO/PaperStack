## Welcome to PaperStack!

[Click here to open PaperStack in Colab.](https://githubtocolab.com/EigenFlowIO/PaperStack/)

### What is PaperStack?
PaperStack is a **multi-agent** AI pipeline designed for automated document generation. It showcases how specialized AI agents can collaborate to create **structured**, **domain-specific** writing, such as **research papers**, **technical reports**, and **formal documents**.

This project is an **experiment** in automation rather than an attempt to replace human-quality academic work or create writing that subverts AI detection. It offers a **transparent** and **modular** approach to observing and refining AI-generated structured content. All outputs are fully AI-generated and not attributable to any individual or entity.

---

### How It Works

#### 1. User Input
The user provides a topic, and the AI pipeline systematically progresses through a sequence of tasks to generate, refine, and format the document.

#### 2. AI Pipeline Overview
PaperStack follows a structured multi-agent workflow to ensure systematic content generation:

- **Task-Specific System Prompts:**  
  Each AI agent is assigned a specialized role with structured prompts tailored to its function, ensuring focused execution at every stage.

- **Strict Formatting Guidelines for Outputs (JSON):**  
  All output content adheres to standardized JSON formatting, maintaining consistency and ensuring compatibility for further processing.

- **Dual-Layer JSON Validation:**  
  Generated JSON responses undergo automated validation to check for structural and syntactical correctness. If parsing fails, a JSON-fixing agent corrects errors until a valid response is achieved.

- **Drafting and Paragraph-Level Revisions:**  
  The system first drafts the document and then performs paragraph-by-paragraph revisions to enhance clarity, coherence, and logical flow.

- **Section Scanning and Coherence Revisions:**  
  Each section undergoes analysis for coherence and redundancy. A separate AI agent ensures logical consistency and minimizes repetition.

- **Attribution Scanning and Citation Insertion:**  
  The system scans for statements requiring attribution and inserts citations in a structured format.

- **Abstract Generation:**  
  A summarization step creates a concise abstract that distills the core arguments and conclusions of the document.

- **Formatting for Printing:**  
  The final document is structured for readability and prepared for output in a format suitable for review.

---

## Future Work

- **Clean and revise initial codebase.**  
- **Add more fields for user inputs, including:**  
  - Additional context to guide the AI's understanding  
  - Additional fields of study  
  - Key points or arguments the user wants included  
  - User prompted hypotheses, methodology, data, and results  
  - Specific philosophers or works to reference  
  - Writing style preference (academic, accessible, narrative)  
- **Include tools for quality analysis, such as:**  
  - Cosine Similarity of Consecutive Sentences  
  - Lexical Overlap Score  
  - N-gram Repetition Count  
  - Compression Ratio  
  - TF-IDF Similarity per Paragraph  
  - Sentence Cohesion Score  
  - Lexical Chain Analysis  
  - Discourse Connective Count  
  - Topic Flow Consistency (TF-IDF Shift)  
  - Entity Grid Model  
- **Refine and improve attribution scanning.**  
- **Link to a database of works like Google Scholar and field-specific OAI-PMH databases to validate works cited.**


---

### Getting Started

#### Step 1: Get Your API Key
PaperStack requires a **Together AI API Key** to generate content using the `Llama-3.3-70B-Instruct-Turbo-free` model.

1. Visit [Together AI](https://together.ai) and sign up or log in.
2. Navigate to **API Keys** in your account settings.
3. Click **Generate New Key**, then copy it.

#### Step 2: Store Your API Key in Google Colab
1. In the left sidebar menu, click the **key icon**.
2. Click **"Add a new secret"**.
3. In the **"Name"** field, enter:  
   ```TogetherAPI```
4. In the **"Value"** field, paste your API key.
5. Toggle **"Notebook access"** to **ON**.

##### API Key Security Measures:
- API keys are **never** displayed in outputs or stored in the notebook.
- If the notebook is **copied, shared, or downloaded**, API keys do not transfer.
- Once stored using **Colab Secrets**, API credentials remain accessible within the notebook without requiring re-entry.

For more details, refer to: [How to Use Secrets in Google Colab](https://medium.com/@parthdasawant/how-to-use-secrets-in-google-colab-450c38e3ec75).

#### Step 3: Initialize
1. Press the **play button** in the upper left corner of this cell to install Together and import necessary libraries.

#### Step 4: Generate the Paper
1. **Enter the topic or title** of the document.
2. Press the **play button** to initiate document generation.
   - **Processing time:** 8-12 minutes.
   - **Note:** Be patient as the system works through the AI pipeline.

---

### Enjoy using PaperStack to streamline your document generation process!
