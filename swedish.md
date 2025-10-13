### Main resources

  * NST speech database https://huggingface.co/datasets/KTH/nst
  * KBLab database rikvox and models https://huggingface.co/KBLab
  * Eurospeech https://huggingface.co/datasets/disco-eth/EuroSpeech
  * Granary dataset

### Many ASR models

  * https://github.com/rhasspy/sv_kaldi-rhasspy
  * https://huggingface.co/jimregan/kaldi-sprakbanken_swe
  * https://huggingface.co/KBLab/kb-whisper-large
  * https://huggingface.co/Banafo/Kroko-ASR (supports Swedish)
  * https://huggingface.co/nvidia/parakeet-tdt-0.6b-v3

### TextCorpora

  * Fineweb2
  * Opensubtitles

Lexicon is part of NST database


### ASR results

WER results

|                           | Common Voice | Fleurs | NST Test | Podcasts |
|---------------------------|--------------|--------|----------|----------|
| KBLab Whisper Large       | 3.9          |  5.0   |  1.6     |  14.5    |
| KrokoASR SV               | 8.0          |  11.1  |  6.0     |  14.5    |
| Whisper V3 Large          | 8.7          |  7.7   |  8.2     |  16.5    |
| Whisper V3 Turbo          | 13.8         |  8.6   |  8.8     |  17.2    |
| Nemo Parakeet 0.6 B V3    | 18.5         | 16.7   |  26.7    |  17.4    |  
| Vosk Large                | 25.6         |  20.7  |  4.8     |  18.4    |
| Vosk Small                | 32.2         | 30.5   |  12.7    |  25.1    |
| Vosk Rhasspy              | 28.6         | 35.4   |  13.2    |  28.8    |
