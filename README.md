# La Roche-Posay RAG Ad Generator

## Personalized Skincare Advertising with RAG

This project implements a lightweight Retrieval-Augmented Generation (RAG) pipeline to generate personalized skincare advertisements for La Roche-Posay products.

The system retrieves product descriptions from a structured knowledge base and combines them with customer skincare profiles to generate targeted marketing content using GPT-4o.

---

## Project Goal

Modern consumers expect personalized marketing experiences. This project demonstrates how a RAG workflow can improve AI-generated advertising by grounding responses in real product information instead of relying solely on general LLM knowledge.

The goal of the system is to:
- Generate personalized skincare advertisements
- Improve relevance using contextual retrieval
- Demonstrate practical applications of Generative AI in marketing

---

## Business Value

This project demonstrates how Generative AI can support personalized marketing by dynamically generating customer-specific advertisements using contextual product retrieval.

The system highlights how RAG pipelines can improve:
- Marketing personalization
- Customer engagement
- Product recommendation quality
- Relevance and factual grounding of AI-generated content

---

## Data Sources

Product descriptions were sourced from La Roche-Posay’s official website.

Products included:
- Retinol B3 Pure Retinol Serum
- Effaclar Multi-Target Acne Treatment
- Anthelios Ultra Light Fluid Facial Sunscreen SPF 60
- Toleriane Double Repair Face Moisturizer

---

## System Design

The project uses a simple Retrieval-Augmented Generation (RAG) workflow:

1. Load product descriptions from JSON knowledge files
2. Accept a customer skincare profile
3. Retrieve relevant product context
4. Inject retrieved context into a prompt
5. Generate personalized advertisements using GPT-4o

---

## RAG Workflow

```text
Customer Profile
       ↓
Product Retrieval (JSON Knowledge Base)
       ↓
Prompt Construction
       ↓
GPT-4o Generation
       ↓
Personalized Advertisement
```

---

## Example User Profiles

Example customer profiles used during testing:
- 40-year-old concerned with wrinkles and aging
- College student with acne and oily skin
- Man in his 30s starting a skincare routine
- Customer with sensitive and dry skin

---

## Example Output

> "Revitalize and renew your skincare routine with Retinol B3 Pure Retinol Serum. Designed to smooth fine lines and improve skin texture, this dermatologist-tested formula combines pure retinol and vitamin B3 for visible anti-aging results."

The system generated multiple advertisement variations tailored to each customer profile.

---

## Key Insight

Using Retrieval-Augmented Generation (RAG) significantly improved output relevance and personalization compared to prompting GPT-4o without product context.

Grounding the model with retrieved product information produced:
- More accurate product recommendations
- Better alignment with skincare concerns
- More realistic marketing language
- Improved consistency across generated outputs

---

## Skills Demonstrated

- Retrieval-Augmented Generation (RAG)
- Prompt Engineering
- Context Injection
- AI-Powered Personalization
- NLP Workflows
- LLM Application Development
- Generative AI Marketing Applications

---

## Technologies Used

- Python
- LangChain
- OpenAI GPT-4o
- JSON Knowledge Base
- Jupyter Notebook
- Retrieval-Augmented Generation (RAG)

---

## Repository Structure

```text
la-roche-posay-rag-ad-generator/
│
├── data/
│   ├── Anthelios_doc_1.json
│   ├── Effaclar_doc_2.json
│   ├── Retinol_B3_doc_3.json
│   └── Toleriane_doc_4.json
│
├── notebooks/
│   └── skincare_rag_generator.ipynb
│
├── images/
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

## Installation

```bash
pip install -r requirements.txt
```

---

## Future Improvements

- Integrate vector databases for semantic retrieval
- Add embedding similarity search
- Build a web application interface
- Expand the product knowledge base
- Add user profile memory and recommendation history
- Deploy as an interactive AI skincare assistant

---

## Author

Christine Whelan  
MS in Artificial Intelligence
