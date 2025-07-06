
# GPT Tokenizer from Scratch 🧠🔤

A hands-on implementation of a **GPT-style tokenizer** using Byte Pair Encoding (BPE), built from scratch in Python — inspired by [@AndrejKarpathy](https://www.youtube.com/@AndrejKarpathy)'s walkthrough on how GPT tokenization works.

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
 
## 📚 References

- [@AndrejKarpathy – YouTube](https://www.youtube.com/@AndrejKarpathy)
- [Karpathy’s minBPE GitHub](https://github.com/karpathy/minbpe)
- [OpenAI's tiktoken GitHub](https://github.com/openai/tiktoken)
- [LessWrong: Anomalous Tokens in GPT](https://www.lesswrong.com/posts/ChtGdxk9mwZ2Rxogt/smartyheadercode-anomalous-tokens-for-gpt3-5-and-gpt-4-1)

## 📬 Contact

Made with curiosity by [Jayant Bisht](https://github.com/jayant1554)

## 🏷 Tags

`#GPT` `#Tokenizer` `#BPE` `#LLM` `#DeepLearning` `#Python` `#FromScratch` `#Colab` `#NLP`
