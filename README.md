# smart-research-assistant

Prototype that summarizes technical articles and answers questions about them, comparing three transformer models.

**What's Inside**

1. Load and explore a dataset of tech articles (title + full text)
2. Summarization & Q&A functions built with:
   *FLAN-T5-Large (encoder-decoder) — limited by a 512-token input cap, leading to repetitive summaries on long articles
   *TinyLlama-1.1B-Chat (decoder-only) — coherent summaries and grounded Q&A on longer text
   *Qwen2.5-3B-Instruct — best overall, tested on both seen and unseen articles
3. Model comparison table (summarization/QA quality, long-article handling)

**Key Takeaway**

Smaller/older models like FLAN-T5 struggle with long inputs and multi-part prompts;
TinyLlama and Qwen2.5 handle longer context better. Breaking complex queries into smaller, focused prompts improves output quality.
