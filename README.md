# AI Finance Automation Platform

A personal finance automation project I built using n8n, OpenAI and various APIs. The goal was to automate some of the repetitive parts of tracking and reviewing my finances.

## What it does

### 1. AI Transaction Parser

Automatically processes banking notification emails and uses OpenAI to extract the transaction details. The workflow then categorises the transaction as an expense or income, records it in Google Sheets, and sends a notification through Telegram.

### 2. AI Finance Assistant

An AI assistant that lets me ask questions about my financial data using natural language. It retrieves the relevant data from Google Sheets and uses OpenAI to generate a response.

### 3. Daily Finance Summary

A scheduled workflow that runs at 9 PM, retrieves recent expense data, generates a spending summary using AI, and sends it to Telegram.

## Tech Stack

- n8n
- OpenAI API
- Python
- Gmail API
- Google Sheets API
- Telegram Bot API

## Workflow Overview

```text
Gmail
  ↓
n8n
  ↓
OpenAI
  ↓
Process transaction
  ↓
Google Sheets
  ↓
Telegram
```

## Repository Structure

```text
workflows/
├── Finance AI Parser
├── Finance Assistant
└── Daily Finance Summary
```

## Note

The workflow files have been sanitised before being uploaded here. Personal information, credentials and private configuration have been removed or replaced with placeholders.

If you want to run the workflows yourself, you will need to connect your own credentials and configure the required services in n8n.
