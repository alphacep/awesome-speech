## TTS voices and systems

  * Piper Turkish voices (many of them)
  * https://huggingface.co/marduk-ra/F5-TTS-Turkish
  * https://huggingface.co/umarigan/speecht5_tts_tr_v1.0
  * https://huggingface.co/Karayakar/Oute-TTS-500M
  * https://huggingface.co/omersaidd/tts_mazlum_kiper_tur_001
  * https://huggingface.co/hcsolakoglu/Orkhon-TTS
  * https://huggingface.co/omersaidd/tts_mazlum_kiper_tur_001
  * https://huggingface.co/Anilosan15/Dia-1.6B-tr
  * https://huggingface.co/Anilosan15/kani-tts-400m-0.3-tr
  * https://huggingface.co/ResembleAI/chatterbox
  * https://huggingface.co/Karayakar/Orpheus-TTS-Turkish-PT-5000

## TTS datasets

  *  Yodas/Emilia
  * https://huggingface.co/datasets/erenfazlioglu/turkishvoicedataset
  * https://huggingface.co/datasets/omersaidd/tts_mazlum_kiper_tur
  * https://huggingface.co/datasets/omersaidd/tts_nisan_kumru_tur (and more)
  * https://huggingface.co/datasets/Anilosan15/Turkish_TTS_Data
  * https://huggingface.co/datasets/kadirnar/combined-turkish-datasets ???
  * https://huggingface.co/datasets/cubukcum/TurkishVoiceDataset (243k Youtube crawl)
  * https://huggingface.co/datasets/Codyfederer/tr-podcast-dataset

# Notable accounts

  * https://huggingface.co/Anilosan15
  * https://huggingface.co/Karayakar
  * https://huggingface.co/kadirnar

## Normalization

Turkish has two distinct letters - i and ı. The problem is that lowercase() doesn't really work for them (it produces extra symbol). A special  replacement is required for text processing.
