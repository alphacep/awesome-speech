Turkic language with quite variable accents from different regions

### Datasets

   * CommonVoice
   * UzbekVoice
   * ISSAI UZ
   * Fleurs
   * https://huggingface.co/islomov/datasets  (youtube, podcasts, it)

## Notable models

   * https://huggingface.co/islomov/rubaistt_v2_medium (whisper medium, recommended)
   * https://huggingface.co/ai-sage/GigaAM-Multilingual
   * Vosk (ok model for the size)
   * https://huggingface.co/rifkat/uzbek-stt-v2 (good wav2vec with LM)
   * https://huggingface.co/Kotib/uzbek_stt_v1 (another whisper)
   * https://huggingface.co/nvidia/stt_uz_fastconformer_hybrid_large_pc (fast conformer)
   * Omnilingual 7B V2 https://github.com/facebookresearch/omnilingual-asr
   * MMS 1B + Rifkat LM (above) https://github.com/facebookresearch/fairseq/tree/main/examples/mms
   * ROVER (Rubai + Giga + Rifkat + Kotlib + Nemo)

## WER

|                               | CV    | Digits  | Fleurs  |  ISSAI | ISSAI Rare |
|------------------------------|--------|---------|---------|---------|-----------|
|         Vosk Small 0.24      | 13.6   | 42.4    |   29.1  |   13.9  | 24.19     |
|         MMS1B + LM           |  17.2  | 80.1    |   21.0  |   28.2  | 43.40     |
| Omnilingual LLM 7B V2        |  20.7  | 57.9    |   16.4  |   29.3  | 45.44     |
|   Nvidia Fastconformer       |  8.9   | 57.5    |   14.9  |   14.4  | 28.85     |
| Rifkat STT v2 (wav2vec + LM) |   6.5  | 28.0    |   23.5  |   7.7   | 21.75     |
| Whisper Medium Kotib         |  8.9   | 9.7     |   13.4  |   14.0  | 33.42     |
| **Whisper Medium Rubai**     |  8.5   | 10.0    |   10.6  |   12.1  | 31.73     |
| GigaAM Multilingual          |  7.24  | 46.79   |  17.44  |   11.30 | 29.58     |
| GigaAM Multilingual Large    |  5.52  | 38.95   |  14.42  |   8.77  | 26.40     |
|------------------------------|--------|---------|---------|---------|-----------|
| Rover                        |  4.60  | 10.13    |  11.20 |   7.05  | 21.80     |

