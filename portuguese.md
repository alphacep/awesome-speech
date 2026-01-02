## WER

|                           | Calls  | CORAA   | CV      |  Fleurs |
|---------------------------|--------|---------|---------|---------|
|         Vosk Small 0.3    | 69.2   | 68.9    |   32.5  |   22.2  |
|         Vosk FB v0.0.1    | 70.1   | 54.2    |   37.1  |   17.2  |
|         Vosk 0.18 Private | 28.9   | 67.8    |   41.6  |   27.0  |
|         Parakeet V3       | 32.2   | 26.6    |    6.6  |   5.1   |
|         Whisper V3 Turbo  | 34.2   | 30.5    |    5.9  |   4.4   |
|         Kroko PT 128L     | 28.2   | 24.2    |    3.7  |   5.4   |
|         FunASR Nano       | 148.7  | 87.1    |   24.4  |   20.3  |
|         Rover             | 24.8   | 22.8    |    4.0  |   4.1   |

Rover = Kroko + Parakeet + Vosk (calls) or Kroko + Parakeet + Whisper (other)

## Other datasets to try

MTEDX <https://www.openslr.org/100/>
Granary <https://huggingface.co/datasets/nvidia/Granary>
