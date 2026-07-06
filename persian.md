## Speech recognition models

### Notable models

  * Vosk <https://alphacephei.com/vosk/models>
  * <https://huggingface.co/Reza2kn/Shenava-Koochik-v1.0>
  * <https://huggingface.co/Reza2kn/Shenava-Rizeh-v1.0>
  * <https://huggingface.co/Reza2kn/Shenava-Rizeh-Pizeh-v1.0>
  * <https://huggingface.co/Neurai/NeuraSpeech_900h>
  * <https://huggingface.co/Peacockery/omni-ctc-300m-farsi>

Other historical models

  * <https://huggingface.co/manifoldix/xlsr-fa-lm>
  * <https://huggingface.co/Neurai/NeuraSpeech_WhisperBase>
  * <https://modelscope.cn/models/iic/speech_UniASR_asr_2pass-fa-16k-common-vocab1257-pytorch-online>
  * <https://huggingface.co/steja/whisper-large-persian>
  * <https://huggingface.co/nvidia/stt_fa_fastconformer_hybrid_large>
  * <https://huggingface.co/m3hrdadfi/wav2vec2-large-xlsr-persian-v3>
  * <https://huggingface.co/makhataei/Whisper-Small-Ctejarat>
  * <https://huggingface.co/hezarai/whisper-small-fa>
  * <https://huggingface.co/vargha/whisper-large-v3-tuned-Persian>
  * <https://github.com/areffarhadi/persian-asr>
  * <https://huggingface.co/aictsharif> - Whisper Base/Small/Tiny/Large, for example <https://huggingface.co/aictsharif/whisper-tiny-fa>


## Notable people

  * <https://huggingface.co/Reza2kn>
  * <https://github.com/mah92>
  * <https://huggingface.co/Peacockery>
  * <https://github.com/MahtaFetrat>

### ASR datasets (testing)

 * [Common Voice 17.0](https://huggingface.co/datasets/mozilla-foundation/common_voice_17_0)
 * [Fleurs](https://huggingface.co/datasets/google/fleurs)
 * Meetings (internal)
 * <https://huggingface.co/datasets/Reza2kn/visualears-golden-6669>

Many existing Persian datasets here

  * <https://huggingface.co/datasets/Reza2kn/persian-asr-text-2.69M-deduped>

To process

  * <https://huggingface.co/datasets/Reza2kn/persian-asr-relabeled-gemini>

### ASR results

WER results

| Model             | Common Voice | Meetings | Fleurs | Visualears |
|-------------------|-------------:|---------:|--------:|-------------
| Vosk 0.42         |         16.7 |     37.9 |   11.1  |     14.4    |
| Vosk Small 0.42   |         23.4 |     43.6 |    14.0 |      19.20  |
| Nemo FC           |         16.2 |     60.6 |    43.8 |         -   |
| Neuro FC          |         24.6 |     51.2 |    23.7 |      32.04  |
| Neuro Whisper     |         23.5 |     45.4 |    25.3 |        -    |
| Manifoldix XLS-R  |         29.5 |     46.0 |    24.5 |        -    |
| Peacock Omni 300M |         23.1 |     33.33|    13.81 |     9.09   |
|Reza2kn Koochik 1.0|     **13.26**| **32.36**|  **9.44**|    **8.11**|


### CER results

| Model             | Common Voice | Meetings | Fleurs | Visualears |
|-------------------|-------------:|---------:|--------:|-------------|
| Vosk 0.42         |          5.7 |     18.7 |    4.0 |     3.90    |
| Vosk Small 0.42   |          8.7 |     22.4 |     5.1 |    5.78    |
| Nemo FC           |      **3.3** |     40.1 |    27.2 |      -     |
| Neuro FC          |          7.6 |     26.0 |     9.0 |       9.53 |
| Neuro Whisper     |          6.8 |     23.0 |     6.7 |     -      |
| Manifoldix XLS-R  |          7.7 |     17.9 |     6.5 |      -     |
| Peacock Omni 300M |          5.7 | **12.86**|    5.10 |   **2.18** |
|Reza2kn Koochik 1.0|          4.08 |   13.42|    **3.35** |   2.65   |

Nemo is overtrained on Common Voice

## Text to speech models

  * <https://github.com/tihu-nlp/tihu>
  * <https://github.com/karim23657/Persian-tts-coqui>
  * <https://huggingface.co/gyroing/Persian-Piper-Model-gyro>
  * <https://github.com/SadeghKrmi/pertts-streamlit> - web interface for Piper voices
  * <https://github.com/Adibian/Persian-MultiSpeaker-Tacotron2>
  * <https://github.com/AlisterTA/Persian-text-to-speech>
  * <https://huggingface.co/Thomcles/Chatterbox-TTS-Persian-Farsi>
  * <https://github.com/MahtaFetrat/Piper-with-LCA-Phonemizer>

## Dictionaries and G2P

  * <https://huggingface.co/datasets/MahtaFetrat/KaamelDict> - 120k entries
  * <https://github.com/tihu-nlp/tihudict> - 47k entries (big) 2k (demo)

  ## G2P converters

  * <https://github.com/AdolfVonKleist/Phonetisaurus>  - when trained on Kaamel PER 3.8%, WER 21.9%
  * <https://github.com/mohamad-hasan-sohan-ajini/G2P> - no pretrained model
  * <https://github.com/PasaOpasen/PersianG2P> - PER 21.6% WER 62%
  * <https://github.com/AzamRabiee/Persian_G2P> - same as above, just refactored code and same checkpoint file
  * <https://github.com/sajadalipour7/Persian-Grapheme-To-Phoneme-With-Transformer> - PER 14.4%, WER 62.5%
  * <https://github.com/de-mh/persian_phonemizer> - phonemizer with POS tagger

  ## Online resources

  * <https://www.peykaregan.ir/dataset>
  * <https://www.wiktionary.org>
  * <http://farhang.apll.ir>

  ### Notes

  Overall, Persian phoneset is more or less stable across packages. Subtle differences:
  
  * Tihu dictionary has some rare phones like '_' and '^' the purpose of which is unknown.
  * Glottal stop affects prosody but doesn't really have acoustic realization in fast speech, so it is removed in HMM models (Vosk). It is still beneficial to keep it in neural models (TTS)
  * PersianG2P predictor is based on RNN and vulnerable to hallucinations, so not really perfect. Also, the Tihu dataset is small. WFST predictor like Phonetisaurus much more accurate even the algorithm is simple by using bigger dataset.
  * Overall, more advanced model trained on Kaamel would perform much better (transformer)
  * Kaamel dictionary has separate phoneme IPA sound 'ɡ' (u0x261) as opposed to 'g'. Not very frequent and purpose is unknown.
  * Kaamel dictionary is most complete but has questionable entries as well

## Normalization

No established code here but here are some variants

  * <https://github.com/roshan-research/hazm>

Others

  * <https://github.com/haraai/ParsiNorm>
  * <https://github.com/ICTRC/Parsivar>
  * <https://github.com/5j9/num2fawords>
  * [Shenhasa Cleanup](https://github.com/shenasa-ai/speech2text/blob/master/language_model/clean_text.py)
  * [Nemo Cleanup](https://huggingface.co/nvidia/stt_fa_fastconformer_hybrid_large)
  * https://github.com/persian-tools/persian-tools - Javascript

  ### Notes

  There is "Colloquial Persian" which is somewhat different from spoken Persian. Yet to find the package to convert between them.

  Persian literate language uses zero-width-non-joiner (u200c) for many words an the patterns to apply it are non-regularand some people expend it to present in recognized texts. Web texts of course do not have it.

## Other awesome lists for Persian

  * <https://github.com/mhbashari/awesome-persian-nlp-ir>
  * <https://github.com/karim23657/awesome-Persian-Speech>
