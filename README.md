# HFT: High Frequency Tokens for Low-Resource NMT

**H**igh **F**requency **T**okenizer is a new subword segmentation algorithm developed to address the issue of low frequency tokens in the training data for Neural Machine Translation systems.

For updated version see the main HFT repo at https://github.com/pary42/hftoks

## Usage

To use `hft`, the input data must be pretokenized with: 

`pretokenize INTEXTFILE > OUTTEXTFILE`. 

To learn a token vocabulary use:
`hftoks.py learn INTEXTFILE OUTVOCABFILE [VOCAB_SIZE [STEP_SIZE]]'`

And then to tokenize your data:
`hftoks.py tokenize VOCABFILE < INTEXT > OUTTOKENS'`

## Cite

> Edoardo Signoroni and Pavel Rychlý. 2022. HFT: High Frequency Tokens for Low-Resource NMT. In Proceedings of the Fifth Workshop on Technologies for Machine Translation of Low-Resource Languages (LoResMT 2022), pages 56–63, Gyeongju, Republic of Korea. Association for Computational Linguistics.

> @inproceedings{signoroni-rychly-2022-hft,
    title = "{HFT}: High Frequency Tokens for Low-Resource {NMT}",
    author = "Signoroni, Edoardo  and
      Rychl{\'y}, Pavel",
    booktitle = "Proceedings of the Fifth Workshop on Technologies for Machine Translation of Low-Resource Languages (LoResMT 2022)",
    month = oct,
    year = "2022",
    address = "Gyeongju, Republic of Korea",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2022.loresmt-1.8",
    pages = "56--63",
    abstract = "Tokenization has been shown to impact the quality of downstream tasks, such as Neural Machine Translation (NMT), which is susceptible to out-of-vocabulary words and low frequency training data. Current state-of-the-art algorithms have been helpful in addressing the issues of out-of-vocabulary words, bigger vocabulary sizes and token frequency by implementing subword segmentation. We argue, however, that there is still room for improvement, in particular regarding low-frequency tokens in the training data. In this paper, we present {``}High Frequency Tokenizer{''}, or HFT, a new language-independent subword segmentation algorithm that addresses this issue. We also propose a new metric to measure the frequency coverage of a tokenizer{'}s vocabulary, based on a frequency rank weighted average of the frequency values of its items. We experiment with a diverse set of language corpora, vocabulary sizes, and writing systems and report improvements on both frequency statistics and on the average length of the output. We also observe a positive impact on downstream NMT.",
}
