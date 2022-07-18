# HFT: High Frequency Tokens for Small Datasets (working title)

**H**igh **F**requency **T**oken(izer) is a new subword segmentation algorithm developed to address the issue of low frequency tokens in the trainig data for Neural Machine Translation systems.

Description TBA

## Usage

To use `hft`, the input data must be pretokenized with: 

`pretokenize INTEXTFILE > OUTTEXTFILE`. 


To learn a token vocabulary use:
`hftoks.py learn INTEXTFILE OUTVOCABFILE [VOCAB_SIZE [STEP_SIZE]]'`

And then to tokenize your data:
`hftoks.py tokenize VOCABFILE < INTEXT > OUTTOKENS'`


## Cite (hopefully)

Signoroni and Rychly, "HFT: High Frequency Tokens for Low-Resource NMT", ...