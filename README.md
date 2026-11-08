# Supplier Offer Comparison

I built this n8n workflow to collect supplier offers, compare them using price, delivery time, and supplier rating, and use AI to prepare a final recommendation.

<img width="745" height="237" alt="Supplier Offer Comparison workflow demo" src="https://github.com/user-attachments/assets/0e469ff0-e8ab-46c1-b6a6-993487c51e23" />

## How it works

1. A user submits a supplier's name, price, delivery time, rating, and RFQ ID through a form.
2. Each submitted offer is saved to Google Sheets, and the workflow retrieves the available offers.
3. JavaScript calculates a score for each offer using price (40%), delivery time (30%), and supplier rating (30%), then ranks the results.
4. Google Gemini reviews the ranked offers and recommends a supplier with an explanation and any concerns.
5. The comparison report is sent by email with the recommendation and offer details.

## Main features

- Supplier offer submission form.
- Weighted scoring based on price, delivery time, and rating.
- Automatic offer ranking.
- AI-generated supplier recommendation.
- Email report with the ranking and comparison details.

## Technologies

n8n, Google Sheets, Google Gemini, JavaScript, AI Agent, Gmail, and n8n Forms.

## Setup

Import [workflow.json](./workflow.json) into n8n, configure your Google Sheets, Gemini, and Gmail credentials, then connect your supplier offers sheet and test the workflow with several sample offers.
