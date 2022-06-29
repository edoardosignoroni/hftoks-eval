#Ideas already explored in papers: mainly voc_size...
.they study BPE and class imbalance, we want to study BPE voc size and efficiency and optimal settings for BLEU, also BLEU score variance across training runs

#Alternatives for LoResMT:
	.dataset
	.evaluation of existing tools

#Frequency in en 30k

0< = 3933 12.87%
10< = 16761
100< = 19846 65.02%

#Speed vs voc size

tokenization speed depends on voc size

en_30k = 25 min
en_10k = 12 min
en_1k = 1.5 min
