Useful teams and people

  * https://huggingface.co/muhtasham
  * https://huggingface.co/Peacockery

Datasets

  * https://huggingface.co/datasets/google/fleurs
  * https://huggingface.co/datasets/Peacockery/tajik-asr-corpus-v3
  * https://huggingface.co/datasets/muhtasham/tajik-asr

and finetuned models

  * https://huggingface.co/alphacep/vosk-model-tg
  * https://huggingface.co/Peacockery/omni-ctc-300m-tajik
  * https://huggingface.co/Peacockery/tajik-parakeet-tdt-110m
  * https://huggingface.co/muhtasham/whisper-non-verbal-new-aug-low-lr-fixed
  * https://huggingface.co/burhon97/whisper-tajik-finetuned

WER results

| Model                              | FLEURS WER | YouTube WER | Telephony WER | Noisy WER |
|------------------------------------|-----------:|------------:|--------------:|----------:|
| Omni CTC 300M                      | 19.90      | 60.97       |     86.54     |           |
| Omni LLM 7B v2                     | **10.59**  | 37.20       |     69.65     |           |
| Omni Peacockery 300M               | 17.94      | 37.58       |     68.14     |           |
| Nemo Fastconformer Peacockery 110M | 18.68      | 33.37       |     65.81     |           |
| Whisper burhon97                   | 14.21      | 45.64       |     69.65     |           |
| Whisper muhtasham                  | 18.04      | 62.27       |     94.49     |           |
| Vosk GigaAM Multilingual Finetune  | 12.73      | 29.54       |     47.57     |  107.54   |
| Vosk tg 0.61                       | 13.85      | 28.21       |     54.28     |           |
| Vosk tg 0.63                       | 12.45      | 27.74       |     43.69     |  49.13    |
| ROVER                              | 11.15      | **26.60**   |   **41.45**   | **42.17** |
