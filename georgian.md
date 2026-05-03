Underresourced language, only CV (160 hours) and Fleurs (tiny) datasets around.

## Interersting links

   * [NVIDIA model training](https://developer.nvidia.com/blog/developing-robust-georgian-automatic-speech-recognition-with-fastconformer-hybrid-transducer-ctc-bpe). The model
     itself is good, but feels overbiased to CV dataset.
   * <https://huggingface.co/NMikka> finetuning all major TTS (OmniVoice, Kokoro, etc). Good finetuned models but dataset needs more work

## ASR accuracy results

|                             | CV  | Fleurs |
|-----------------------------|-----|--------|
|         Vosk Small          | 14.2 | 18.0  |
|         Vosk Large          |  5.2 | 12.7  |
|         Nemo Fastconformer  |  3.7 | 14.6  |
|         Omnivoice 300M LLM  | 11.7 | 17.7  |
|         Omnivoice 7B   LLM  |  6.4 | 12.3  |
