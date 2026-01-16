Turkic language with quite variable accents from different regions

### Datasets

   * CommonVoice
   * UzbekVoice
   * ISSAI UZ
   * Fleurs

## Notable models

   * Vosk (ok model for the size)
   * https://huggingface.co/rifkat/uzbek-stt-v2 (recommended)
   * https://huggingface.co/Kotib/uzbek_stt_v1
     
   * https://huggingface.co/nvidia/stt_uz_fastconformer_hybrid_large_pc
   * Omnilingual 7B (yet to test for Uzbek)
   * MMS 1B + Rifkat LM (above) https://github.com/facebookresearch/fairseq/tree/main/examples/mms

## WER

|                               | CV    | Digits  | Fleurs  |  ISSAI |
|------------------------------|--------|---------|---------|---------|
|         Vosk Small 0.24      | 13.2   | 54.9    |   29.1  |   13.9  |
|   Nvidia Fastconformer       | 6.9    | 59.5    |   14.9  |   14.4  |
|         MMS1B + LM           |  18.7  | 94.6    |   22.0  |   28.2  |
| Rifkat STT v2 (wav2vec + LM) |   8.3  |  35.9   |   23.5  |   7.7   |
|  Rover                       |   7.0  |    33.9    |   16.4  |   7.4   |

