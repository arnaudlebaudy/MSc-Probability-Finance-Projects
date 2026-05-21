We evaluate different strategies for answering medical flashcards (Medalpaca/medical_meadow_medical_flashcards) without external retrieval.

We start with a closed‑book baseline (cloud OpenAI vs local Llama models), then test a self‑check mechanism. Next we fine‑tune a small model (SmolLM 135M) using LoRA, studying the effect of the prompt, the number of trainable parameters, dataset size, and epochs. Finally we compare advanced prompt engineering techniques on semantic correctness, lexical similarity and inference latency.

Fine‑tuning improves over the base model but stays far behind a large LLM. Prompt engineering can change style drastically but does not always improve semantic accuracy. Lexical metrics (ROUGE, BLEU) are misleading for medical QA ; LLM‑as‑a‑judge is more reliable. Simple prompts offer the best quality‑latency trade‑off.

The report and source code can be provided upon request.

