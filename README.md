# Italian Kaldi Profile

A [Rhasspy](https://github.com/rhasspy/rhasspy) profile for Italian (`it`).

Includes:

* A [Kaldi nnet3](https://kaldi-asr.org/doc/dnn3.html) speech to text model
    * See files in `acoustic_model/`
    * Recipe created with [ipa2kaldi](https://github.com/rhasspy/ipa2kaldi)
    * Trained on:
        * [Common Voice](https://commonvoice.mozilla.org) (129 hours)
        * [M-AILabs](https://www.caito.de/2019/01/the-m-ailabs-speech-dataset/) (128 hours)
* An [IPA](https://en.wikipedia.org/wiki/International_Phonetic_Alphabet) pronunciation lexicon pulled from [Wiktionary](https://www.wiktionary.org/)
    * See `base_dictionary.txt.gz`
* A [phonetisaurus](https://github.com/AdolfVonKleist/Phonetisaurus) grapheme to phoneme model for predicting word pronunciations
    * See `g2p.fst.gz`
    * Trained on `base_dictionary.txt.gz`
* A tri-gram [ARPA language model](https://cmusphinx.github.io/wiki/arpaformat/)
    * See `base_language_model.txt.gz`
    * Text from audio transcriptions, [Common Voice](https://github.com/mozilla/common-voice/tree/master/server/data/it), and [Universal Dependencies](https://universaldependencies.org/)
