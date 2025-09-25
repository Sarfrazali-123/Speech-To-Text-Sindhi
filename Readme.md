# Sindhi ASR — Fine-tuned openai/whisper-tiny

## Overview
This repository describes a fine-tuned automatic speech recognition (ASR) model for Sindhi based on `openai/whisper-tiny`. The model was trained on a small corpus of paired audio–transcription examples and evaluated on a held-out test set.

**Model (base):** openai/whisper-tiny  
**Task:** Speech-to-text (Sindhi)  
**Dataset size (pairs):** 244 audio–transcription pairs  
**Reported metric (Average WER on test set):** 0.8731

---

## Dataset
- Total paired examples used for fine-tuning: **244**
- Language: **Sindhi**
- Audio duration: *not specified* (please add total hours/minutes if available)
- Transcription style: *not specified* (e.g., normalized text, punctuation, casing — please add if available)

⚠️ Because the dataset is small, the model will likely underperform on wide-domain Sindhi audio.  
WER reported on test set: **0.8731** (≈87.31% errors).

---

## Results and interpretation
- **Average WER on test set:** 0.8731  
- High WER may be caused by:
  - Very small dataset size  
  - Acoustic mismatch (different recording conditions)  
  - Limited model capacity (`whisper-tiny` is small)  
  - Data/transcription inconsistencies  

**Next steps to improve:**
- Collect more Sindhi audio (tens to hundreds of hours ideally)  
- Apply data augmentation (speed perturbation, noise, reverberation)  
- Normalize transcripts consistently  
- Try larger models (`whisper-small`, `whisper-medium`)  

---

## Demo and Results

![Alt Text](https://github.com/Sarfrazali-123/Speech-To-Text-Sindhi/blob/ba0e621bd804eb8bcf450380cd7cf2a521d17a2e/Tiny.png)

