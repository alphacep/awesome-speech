A lot of useful models and data were cleaned and created during BengaliAI competition in 2023.

https://bengaliai.github.io

The language is divided between India and Bangladesh and despite claims Kolkata Bangla and Bangladesh Bangla are different in terms of accents, some minor grammar variations and vocabulary. So datasets from both regions have to be collected.

Major efforts to support Bangla ASR:

  * <https://huggingface.co/ai4bharat>
  * <https://huggingface.co/bengaliAI>
  * <https://huggingface.co/SpireLab>
  * <https://huggingface.co/hishab>
  * <https://huggingface.co/SUST-CSE-Speech>

A lot of datasets were recorded and collected, however, datasets are not very diverse, for example not so much telephony data.


### ASR results

WER results

The following datasets used for evaluation:

   * [BanSpeech](https://huggingface.co/datasets/SUST-CSE-Speech/banspeech) - Bangladesh, diverse
   * CommonVoice, Fleurs, IndicTTS, Kathbath, Kathbath Hard - from <https://github.com/AI4Bharat/vistaar>
   * [Respin 2025](https://sites.google.com/view/respinasrchallenge2025) - Indic
   * [Subakko](https://huggingface.co/datasets/SUST-CSE-Speech/SUBAK.KO) - Bangladesh, read speech

We test the following models:

   * <https://huggingface.co/bengaliAI/tugstugi_bengaliai-asr_whisper-medium> - Winner of MaCRo challenge
   * <https://www.kaggle.com/competitions/bengaliai-speech/writeups/qdv206-2nd-place-solution> - Second place with Wav2Vec
   * <https://github.com/AI4Bharat/IndicConformerASR> - latest model from AI4Bharat
   * <https://huggingface.co/hishab/titu_stt_bn_fastconformer> - not well known but good Bangla model

Despite data amounts the WER is still quite high. This is mostly due to lack of proper annotation in training databases. Models are very dialect-dependent.

|                           | CV  | Fleurs | Indic TTS|       Kathbath | Kathbath Noisy | Respin | Subakko | Banspeech |
|---------------------------|-----|--------|----------|----------------|----------------|--------|---------|-----------|
|         IndicConformer BN | 15.7 | 18.1  |   37.5   |         13.3   |     14.9       | 38.1   |   35.1  | 41.1      |
|         Hishab Titu BN    | 29.4 | 39.2  |   53.4   |         31.8   |     33.3       |  45.3  |   34.7  | 38.6      |
|         Tugstugi Whisper  | 12.8 | 17.1  |   22.9   |         12.8   |     15.1       | 13.5   |   21.0  | 28.7      |
|         QDV206 Wav2Vec    | 10.0 | 17.5  |   27.5   |         11.8   |     12.9       | 16.5   |   19.5  | 32.1      |
