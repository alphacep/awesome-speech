Turkic language with quite variable accents

### Datasets

   * CommonVoice
   * UzbekVoice
   * ISSAI UZ

## Notable models

   * Vosk
   * https://huggingface.co/nvidia/stt_uz_fastconformer_hybrid_large_pc
   * https://huggingface.co/rifkat/uzbek-stt-v2
   * https://huggingface.co/Kotib/uzbek_stt_v1
   * Omnilingual 7B (yet to test for Uzbek)
   * MMS 1B

## WER

|                               | CV    | Digits  | Fleurs  |  ISSAI |
|------------------------------|--------|---------|---------|---------|
|         Vosk Small 0.24      | 13.2   | 54.9    |   29.1  |   13.9  |
|   Nvidia Fastconformer       | 6.9    | 59.5    |   14.9  |   14.4  |
|         MMS1B + LM           |    -   |    -    |   22.0  |   -     |
| Rifkat STT v2 (wav2vec + LM) |    -   |    -    |   23.5  |   7.7   |
|  Rover                       |    -   |    -    |   16.4  |   7.4   |

