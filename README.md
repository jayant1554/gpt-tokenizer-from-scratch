
# GPT Tokenizer from Scratch 🧠🔤

A hands-on implementation of a **GPT-style tokenizer** using Byte Pair Encoding (BPE), built from scratch in Python — inspired by [Sam Witteveen's](https://www.youtube.com/@SamWitteveenAI) excellent tutorial ["Let’s Build the GPT Tokenizer"](https://youtu.be/zduSFxRajkE?si=WnplvHI9X3ttASJ5).

This project aims to demystify how GPT and other LLMs process text before feeding it into the model — showing how raw bytes are merged into meaningful tokens through BPE.

## 🔍 Project Goals

- Understand how GPT tokenization works at the byte level
- Implement BPE merging logic manually
- Explore the differences between GPT-2 and GPT-4 tokenization
- Learn why inefficient tokenization can lead to LLM hallucinations

## 🚀 Features

- 🔡 Byte-level UTF-8 encoding of input text
- 🔁 BPE-based token merging (`get_stats`, `merge`)
- 🔧 Custom `encode()` and `decode()` functions
- 🧪 Tests on multilingual and rare tokens
- 📊 Insights on how tokenization affects LLM behavior

## ⚠️ Why Tokenization Matters

In earlier LLMs like GPT-2:
- Words like `SolidGoldMagikarp` were treated as **single tokens** due to training quirks.
- Tokens like `|endoftext|` were baked in and mishandled by some downstream tools.
- This caused hallucinations, incorrect truncation, and context overflow.

GPT-4 improved this by:
- Breaking complex/rare words into meaningful sub-parts.
- Expanding the tokenizer’s efficiency and character support.
- Making better use of the token budget (8192/32k+).

## 🧠 Key Learnings

- Tokenization is not “just preprocessing” — it's how LLMs *see* language.
- Byte Pair Encoding (BPE) is central to vocabulary compression.
- Building from scratch helps understand model context, hallucination triggers, and input optimization.

## 📓 Colab Notebook

👉 [View on Google Colab](https://colab.research.google.com/drive/1y0KnCFZvGVf_odSfcNAws6kcDD7HsI0L?usp=sharing)

## 📚 References

- [Let's Build the GPT Tokenizer – YouTube](https://youtu.be/zduSFxRajkE?si=WnplvHI9X3ttASJ5)
- [OpenAI's tiktoken GitHub](https://github.com/openai/tiktoken)
- [Karpathy: BPE Tokenizer in 100 lines](https://github.com/karpathy/minbpe)
- [LessWrong: Anomalous Tokens in GPT](https://www.lesswrong.com/posts/ChtGdxk9mwZ2Rxogt/smartyheadercode-anomalous-tokens-for-gpt3-5-and-gpt-4-1)

## 📬 Contact

Made with curiosity by [Jayant Bisht](https://github.com/jayant1554)

## 🏷 Tags

`#GPT` `#Tokenizer` `#BPE` `#LLM` `#DeepLearning` `#Python` `#FromScratch` `#Colab` `#NLP`
"""

# Save to file
readme_path = "/mnt/data/README.md"
with open(readme_path, "w", encoding="utf-8") as f:
    f.write(readme_content)

readme_path


