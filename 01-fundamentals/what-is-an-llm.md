# What is an LLM?

📚 **Status: Learning in Progress**

---

## What is an LLM?

LLM stands for **Large Language Model**—a type of AI trained on massive amounts of text to understand and generate human-like responses. Think of it as autocomplete on steroids: instead of just predicting the next word, it can write entire paragraphs, answer questions, summarize documents, or even write code.

Unlike traditional software that follows explicit rules ("if user clicks button, do X"), LLMs predict responses based on patterns learned from billions of text examples. ChatGPT, GitHub Copilot, and Google Bard are all LLMs.

**Key difference:** Traditional software executes instructions. LLMs generate probable responses based on training data.

---

## Key Concepts PMs Must Understand

### Tokens: How Text is Processed

LLMs don't read words—they read **tokens**. A token is roughly 3-4 characters, so "hello world" is about 2-3 tokens.

**Why PMs care:**
- **Cost:** APIs charge per token (input + output). A 1,000-word response costs more than a 100-word one.
- **Performance:** More tokens = slower responses and higher latency.
- **Limits:** Models have maximum token counts (e.g., 4K, 128K tokens).

**Example:** A typical email (~200 words) is roughly 300 tokens. If your product processes 10,000 emails/day, you're using ~3M tokens.

### Context Window: Memory Limitation

The **context window** is how much text the model can "remember" at once—like working memory. A 4K token context means the model only sees the last ~3,000 words of conversation.

**Why PMs care:**
- **Product design:** Long conversations lose early context. Need to decide what to keep vs. discard.
- **Feature limits:** Document Q&A works differently for 5-page vs. 500-page documents.
- **Cost vs. capability:** Larger context windows (128K tokens) cost more but handle longer inputs.

**Product implication:** If building a chatbot for customer support, you need to decide: do you summarize old messages or let context "forget" them?

### Temperature: Creativity Control

**Temperature** (0.0 to 1.0) controls randomness in responses.

- **Low temperature (0.1-0.3):** Consistent, predictable, factual. Same prompt → same answer.
- **High temperature (0.7-1.0):** Creative, varied, less predictable. Same prompt → different answers.

**Why PMs care:**
- **Use case alignment:** Customer support needs low temperature (consistent answers). Creative writing tools need high temperature (varied suggestions).
- **Quality control:** High temperature increases hallucinations (making up facts).

**Example use cases:**
- Low temperature: FAQ bot, data extraction, classification
- High temperature: Marketing copy generation, brainstorming tools, creative writing

---

## Why PMs Should Care

Understanding LLMs helps you:

1. **Scope features realistically:** Know what's possible (summarization, Q&A) vs. what's hard (perfect accuracy, real-time data).

2. **Estimate costs:** Token-based pricing means high-volume features (e.g., analyzing every email) cost differently than low-volume (e.g., monthly reports).

3. **Design better UX:** Understanding context limits helps you design features like "conversation memory" or "document upload limits."

4. **Ask engineers the right questions:** "What temperature are we using?" or "How are we handling context overflow?" shows you understand the tradeoffs.

5. **Manage expectations:** LLMs are probabilistic, not deterministic—they sometimes get things wrong. Design for graceful failures.

**Real product scenario:** Building a document Q&A feature. You need to know:
- How long are typical documents? (impacts context window choice)
- How many queries per user? (impacts cost)
- Do we need exact answers or summaries? (impacts temperature and prompt design)

---

**Last Updated:** 2025-11-22
**Status:** Learning in Progress
