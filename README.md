# la-roche-posay-rag-ad-generator
# Personalized Skincare Advertising with RAG

This project implements a simple Retrieval-Augmented Generation (RAG) system to generate personalized skincare advertisements for La Roche-Posay products.

The system retrieves product descriptions and combines them with customer profiles to generate tailored marketing messages using an LLM.

## Project Goal

Modern consumers expect personalized marketing. This project demonstrates how a RAG pipeline can generate targeted social media advertisements based on user skincare concerns.

## Data Sources

Product descriptions were sourced from La Roche-Posay’s official website.

Products included:

- Retinol B3 Pure Retinol Serum
- Effaclar Multi-Target Acne Treatment
- Anthelios Ultra Light Fluid Facial Sunscreen SPF 60
- Toleriane Double Repair Face Moisturizer

## System Design

The system uses a simple RAG pipeline:

1. Load product descriptions from `.json` and `.txt` files
2. Accept a user skincare profile
3. Inject context and query into a prompt
4. Generate advertisements using GPT-4o

## Example User Profiles

Example profiles used in testing:

- 40-year-old concerned with wrinkles and aging
- college student with acne and oily skin
- man in his 30s starting skincare

## Example Output

> "Revitalize and renew with our anti-aging Retinol Serum. Transform dull skin with the power of pure retinol and vitamin B3."

The system generated multiple variations of each ad tailored to the customer profile.

## Key Insight

Using RAG significantly improved output relevance compared to prompting GPT alone without product context.

## Technologies Used

- Python
- LangChain
- OpenAI GPT-4o
- Retrieval-Augmented Generation (RAG)

## Repository Structure
