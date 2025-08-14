# Cryptocurrency Q/A Dataset Generator
## What I'm Doing Here

I'm building a pipeline to convert unstructured cryptocurrency-related text (articles, videos, books) into structured Q/A pairs in JSON format. This dataset will be used to fine-tune AI models, ensuring they provide accurate, well-structured answers on blockchain and cryptocurrency topics.

## Data Sources
Articles: Scraped from reputable public websites.

Videos: Transcripts extracted from publicly available videos.

Books: Text extracted from purchased books using pdfplumber.

## How It Works
Input: Raw text from articles, videos, or books.

Processing: The text is fed into Deepseek LLM, which generates clear, context-independent Q/A pairs.

Output: Structured JSON with questions, answers, categories, and sources.


## How will the training data look?

```
{
  "questions": [
    {
      "question": "How do Bitcoin miners verify transactions?",
      "answer": "Bitcoin miners verify transactions by solving cryptographic puzzles via proof-of-work consensus.",
      "category": "Blockchain Tech (Consensus)",
      "source": "Bitcoin Whitepaper"
    },
    {
      "question": "What are Ethereum smart contracts?",
      "answer": "Ethereum smart contracts are self-executing agreements written in Solidity that run on the EVM.",
      "category": "Blockchain Tech (Smart Contracts)",
      "source": "Ethereum Documentation"
    }
  ]
}
```
