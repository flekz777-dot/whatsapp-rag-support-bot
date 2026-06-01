# WhatsApp RAG Support Bot

AI-powered WhatsApp support bot with RAG (Retrieval-Augmented Generation) — automatically answers customer questions using a knowledge base.

## Result
**90% of support requests handled automatically** without human intervention.

## How it works

1. Customer sends a message via WhatsApp
2. n8n receives the message through WhatsApp Cloud API webhook
3. Message gets converted to embeddings (vector representation)
4. Supabase Vector DB performs semantic search across the knowledge base
5. Most relevant context is retrieved
6. GPT-4o generates a personalized response based on the context
7. Response is sent back to the customer via WhatsApp

## Tech Stack

| Tool | Purpose |
|---|---|
| n8n | Workflow orchestration |
| WhatsApp Cloud API | Messaging channel |
| Supabase Vector DB | Knowledge base + semantic search |
| OpenAI GPT-4o | Response generation |
| OpenAI Embeddings | Text vectorization |

## Key Features

- **RAG Architecture** — answers based on actual knowledge base, not hallucinations
- **Semantic Search** — finds relevant context even with different wording
- **Error Handling** — fallback to human agent if confidence is low
- **Scalable** — handles multiple conversations simultaneously

## Business Impact

- 90% reduction in first-line support workload
- 24/7 availability without human agents
- Consistent response quality across all conversations
