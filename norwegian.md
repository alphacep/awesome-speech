Norwegian has two branches - Nynorsk and Bokmal, second is "book language" more official. Their relation for ASR/TTS is not yet known for us. Not even sure if they are phonetically different.

Some work on Norwegian happens at NBAILAb

https://huggingface.co/NbAiLab

Not much model published already but there is finetuned whisper.

Parakeet v3 does not support Norwegian.

NST dataset for Norwegian is a good start but resources are limited. Some parlamentary speech and not much youtube.


### ASR results

WER results

|                           | Podcasts     | Fleurs | NST Test |
|---------------------------|--------------|--------|----------|
| Whisper V3 Large          | 16.3         |  8.0   |  12.5    |
| Whisper V3 Turbo          | 15.8         |  8.8   |  13.4    |
| Vosk Large                | 17.2         |  12.3  |  4.3     |
| NBAILab Whisper Turbo     | 24.0         |  8.3   |  13.8    |
| Vosk Small                | 28.6         |  18.0  |  9.5     |
