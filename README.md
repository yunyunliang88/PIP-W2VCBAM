**PIP-W2VCBAM: A deep learning architecture for predicting proinflammatory peptides using Word2Vec-based transformer and CBAM attention**
# Experimental setup
The deep learning framework is operated in Python 3.9 and PyTorch 2.4.1+cpu under PyCharm, and the operating system is 64-bit Windows 10. The hardware environment is AMD Ryzen 5 PRO 4650U with Radeon Graphics 2.10 GHz, and RAM is 16.0 GB.
# Data preprocessing
First, the data in FASTA format is processed into CSV format. Then, short sequences are complemented with virtual amino acid “X” to match the length of the longest sequence using “complementary.py”, resulting in the input datasets “Benchmark_complementary” and “Indtest_complementary”.
# Reproducibility
The results on the independent test set can be reproduced using Indtest_complementary.csv and predict.py, which loads mainmodel.py, the pre-trained model “word2vec.model”, and the saved model “trained PIP-W2VCBAM.pt”.
