# AuraFlow — Multimodal Video Intelligence System

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Mitravinda7/AuraFlow/blob/main/AuraFlow_final_v2.ipynb)

## 🔑 API Keys Setup
This notebook uses Colab Secrets (never hardcoded).

1. Open the notebook in Google Colab
2. Click the 🔑 **Secrets** icon in the left sidebar
3. Add two secrets:
   - `GROQ_API_KEY` → get free key at https://console.groq.com
   - `HF_TOKEN` → get free token at https://huggingface.co/settings/tokens
4. Enable notebook access for both secrets
5. Run cells in order starting from Cell 1


## What it does
- Transcribes video with Whisper + speaker diarization (pyannote)
- Analyzes visual frames with CLIP + LLaMA 3.2 Vision
- Summarizes, chapters, translates, and answers Q&A via Groq LLM
- Fine-tuned RoBERTa sentiment (85%+ accuracy) fused with visual emotion
- Similarity evaluation (auto + manual modes)
- Full Gradio UI with accuracy panel and summary video export

## Setup
1. Run in Google Colab (GPU recommended)
2. Set your API keys in Cell 7:
   - GROQ_API_KEY from https://console.groq.com
   - HF_TOKEN from https://huggingface.co/settings/tokens
3. Run cells in order: Cell 1 → restart → Cell 2 onward

## Tech Stack
Whisper · pyannote · CLIP ViT-L-14 · RoBERTa · LLaMA 3.2 Vision · Groq · FAISS · Gradio
