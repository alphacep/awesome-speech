Turkic language with quite variable accents from different regions

### Datasets

   * CommonVoice
   * UzbekVoice https://huggingface.co/datasets/DavronSherbaev/uzbekvoice
   * ISSAI UZ
   * Fleurs
   * https://huggingface.co/islomov/datasets  (youtube, podcasts, it)
   * https://huggingface.co/datasets/k2speech/FeruzaSpeech
   * https://huggingface.co/instinct-org/collections - some loosely organized data
   * https://huggingface.co/datasets/OvozifyLabs/asr_evaluate_set - evaluation dataset with Telegram messages
   * https://huggingface.co/datasets/openbank-uz/youtube_transcriptions - large autotranscribed dataset (300k rows, gemini transcribed)
   * https://huggingface.co/datasets/Abduqayum/Uzbek-STT-Dataset-780h - dataset from the above, gemini transribed

## Notable models

   * https://huggingface.co/islomov/rubaistt_v2_medium (whisper medium, recommended)
   * https://huggingface.co/ai-sage/GigaAM-Multilingual
   * Vosk (ok model for the size)
   * https://huggingface.co/rifkat/uzbek-stt-v2 (good wav2vec with LM)
   * https://huggingface.co/Kotib/uzbek_stt_v1 (another whisper)
   * https://huggingface.co/nvidia/stt_uz_fastconformer_hybrid_large_pc (fast conformer)
   * Omnilingual 7B V2 https://github.com/facebookresearch/omnilingual-asr
   * MMS 1B + Rifkat LM (above) https://github.com/facebookresearch/fairseq/tree/main/examples/mms
   * https://huggingface.co/collections/navai-uz/navai-whisper-collection - Whisper models from Navai https://navai.pro
   * https://huggingface.co/uzinfocom-edu-ai/asr-uz-fastconformer-large - fastconformer (cv + issai + uzvoice + islomov)
   * https://huggingface.co/Abduqayum/whisper-uzbek-medium-callcenter - whisper with callcenter augmentation
   * ROVER (Rubai + Giga + Rifkat + Kotlib + Nemo)

## WER

| Model                       |    CV | Digits | Fleurs | ISSAI | ISSAI Rare | Feruza |  Ovozify |
|-----------------------------|------:|-------:|--------:|-------:|------------:|--------:|------:|
| Vosk Small 0.24             | 13.59 |  42.42 |   27.34 |  13.94 |       24.19 |       – | 57.81 |
| MMS1B + LM                  | 17.24 |  80.06 |   23.39 |  28.18 |       43.70 |       – |     – |
| Omnilingual LLM 7B V2       | 20.74 |  57.92 |   16.90 |  29.30 |       45.44 |       – |     – |
| Nvidia FastConformer        |  8.86 |  57.49 |   15.10 |  14.37 |       28.85 |    6.61 | 54.56 |
| Vosk 0.60 Streaming         | 10.63 |  25.82 |   18.91 |  16.53 |       37.38 |    9.22 | 49.33 |
| Rifkat STT v2 (wav2vec + LM)|  6.46 |  28.02 |   20.03 |   7.74 |       21.75 |    8.89 | 44.44 |
| Whisper Medium Kotib        |  8.92 |   9.74 |    7.72 |  14.05 |       33.42 |    5.93 | 22.04 |
| Whisper Medium Rubai        |  8.52 |  10.03 |   4.74*|  12.06 |       31.73 |    6.65 | 24.58 |
| Whisper Medium Navai        |  7.28 |  25.95 |   7.64  |  9.21 |       24.42 |    7.64 | 46.06 |
| GigaAM Multilingual         |  7.24 |  46.79 |   11.96 |  11.30 |       29.58 |    6.58 | 23.17 |
| **GigaAM Multilingual Large**|  5.52 |  38.95 |    8.82 |   8.77 |       26.40 |    5.93 | 20.82 |
| **Rover**                   |**4.64**|**11.85**|**5.57**|**7.23**|    **22.27**| **5.15**|**19.88**|

* Likely Rubai Fleurs results are cheating, test included into training
