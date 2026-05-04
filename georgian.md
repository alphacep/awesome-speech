Underresourced language, only CV (160 hours) and Fleurs (tiny) datasets around.

## Interersting links

   * [NVIDIA model training](https://developer.nvidia.com/blog/developing-robust-georgian-automatic-speech-recognition-with-fastconformer-hybrid-transducer-ctc-bpe). The model
     itself is good, but feels overbiased to CV dataset.
   * <https://huggingface.co/NMikka> finetuning all major TTS (OmniVoice, Kokoro, etc). Good finetuned models but dataset needs more work
   * https://github.com/facebookresearch/omnilingual-asr works rather well. V2 version is not very meaningful, only 7B is better, smaller models are worse.

## ASR accuracy results

|                                | CV  | Fleurs |
|--------------------------------|-----|--------|
|         Vosk Small             | 14.2 | 18.0  |
|         Vosk Large             |  5.2 | 12.7  |
|         Nemo Fastconformer     |  3.7 | 14.6  |
|         OmnilingualASR 300M LLM     | 11.7 | 17.7  |
|         OmnilingualASR 7B   LLM     |  6.4 | 12.3  |
|         OmnilingualASR 7B   LLM V2  |  6.6 | 12.1  |
| Rover (Omni 7B V2 + Vosk + Nemo)  |  2.5 |  9.3  |
