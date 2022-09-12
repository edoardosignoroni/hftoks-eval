# HFT: High Frequency Tokens for Low-Resource NMT

**H**igh **F**requency **T**okenizer is a new subword segmentation algorithm developed to address the issue of low frequency tokens in the training data for Neural Machine Translation systems.

We use pretokenization

## Usage

To use `hft`, the input data must be pretokenized with: 

`pretokenize INTEXTFILE > OUTTEXTFILE`. 


To learn a token vocabulary use:
`hftoks.py learn INTEXTFILE OUTVOCABFILE [VOCAB_SIZE [STEP_SIZE]]'`

And then to tokenize your data:
`hftoks.py tokenize VOCABFILE < INTEXT > OUTTOKENS'`


## Cite

> Signoroni and Rychly, "HFT: High Frequency Tokens for Low-Resource NMT", Forthcoming