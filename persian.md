## Speech recognition models

  * Vosk <https://alphacephei.com/vosk/models>
  * <https://huggingface.co/manifoldix/xlsr-fa-lm>
  * <https://huggingface.co/Neurai/NeuraSpeech_900h>
  * <https://huggingface.co/Neurai/NeuraSpeech_WhisperBase>
  * <https://modelscope.cn/models/iic/speech_UniASR_asr_2pass-fa-16k-common-vocab1257-pytorch-online>
  * <https://huggingface.co/steja/whisper-large-persian>
  * <https://huggingface.co/nvidia/stt_fa_fastconformer_hybrid_large>
  * <https://huggingface.co/m3hrdadfi/wav2vec2-large-xlsr-persian-v3>
  * <https://huggingface.co/makhataei/Whisper-Small-Ctejarat>
  * <https://huggingface.co/hezarai/whisper-small-fa>
  * <https://huggingface.co/vargha/whisper-large-v3-tuned-Persian>
  * <https://github.com/areffarhadi/persian-asr>

### ASR datasets (testing)

 * [Common Voice 17.0](https://huggingface.co/datasets/mozilla-foundation/common_voice_17_0)
 * [Fleurs](https://huggingface.co/datasets/google/fleurs)
 * Meetings (internal)

### ASR results

WER results

|              | Vosk 0.5 | Vosk Small 0.5 | Vosk 0.42     | Vosk Small 0.42 | Nemo FC | Neuro FC | Neuro Whisper | Manifoldix XLS-R |
|--------------|----------|----------------|---------------|-----------------|---------|----------|---------------|------------------|
| Common Voice |   29.7   |     31.2       |   16.7        |    23.4         | **16.2**|  24.6    |  23.5         |     29.5         |
| Meetings     |   53.1   |     54.4       |   **37.9**    |    43.6         |  60.6   |  51.2    |  45.4         |     46.0         |
| Fleurs       |   25.1   |     26.2       |   **11.1**    |    14.0         |  43.8   |  23.7    |  25.3         |     24.5         |

CER results

|              | Vosk 0.5 | Vosk Small 0.5 | Vosk 0.42     | Vosk Small 0.42 | Nemo FC | Neuro FC | Neuro Whisper | Manifoldix XLS-R |
|--------------|----------|----------------|---------------|-----------------|---------|----------|---------------|------------------|
| Common Voice |   10.0   |     10.7       |   5.7         |    8.7          |**3.3**  |  7.6     |  6.8          |     7.7          |
| Meetings     |   27.4   |     27.8       |    18.7       |    22.4         |  40.1   |  26.0    |  23.0         |    **17.9**      |
| Fleurs       |   7.0    |      7.5       |   **4.0**     |    5.1          |  27.2   |   9.0    |   6.7         |     6.5          |

Nemo is overtrained on Common Voice

## Text to speech models

  * <https://github.com/tihu-nlp/tihu>
  * <https://github.com/karim23657/Persian-tts-coqui>
  * <https://huggingface.co/gyroing/Persian-Piper-Model-gyro>
  * <https://github.com/SadeghKrmi/pertts-streamlit> - web interface for Piper voices
  * <https://github.com/Adibian/Persian-MultiSpeaker-Tacotron2>
  * <https://github.com/AlisterTA/Persian-text-to-speech>
  * <https://huggingface.co/Thomcles/Chatterbox-TTS-Persian-Farsi>

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
