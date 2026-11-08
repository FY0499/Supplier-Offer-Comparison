# Supplier Offer Comparison

An n8n workflow that collects supplier offers, scores them using price, delivery time, and supplier rating, and uses AI to produce a final recommendation.

## How it works

1. A user submits supplier details, price, delivery days, rating, and an RFQ identifier through a form.
2. The workflow stores each offer in Google Sheets and retrieves the available offers.
3. JavaScript calculates a weighted score using price, delivery time, and supplier rating, then ranks the offers.
4. A Gemini-powered AI agent explains the ranking and recommends a supplier.
5. The final comparison report is sent by email.

## Technologies

- n8n
- Google Gemini
- Google Sheets
- Gmail
- JavaScript
- n8n Forms

## Setup

1. Import workflow.json into n8n.
2. Configure Google Sheets, Gemini, and Gmail credentials.
3. Connect your supplier offers sheet and verify its column names.
4. Submit several offers with the same RFQ identifier to test the comparison.

## Notes

This repository contains the exported n8n workflow. Configure your own credentials and integrations in n8n before running it.
