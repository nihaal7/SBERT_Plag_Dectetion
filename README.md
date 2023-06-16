# Detecting machine-obfuscated content to bypass plagiarism detectors using Sentence BERT-based classifiers

**Authors: Nihaal Subhash, Joshua Levitas, Hanhee Yang**

Paraphrasing tools such as the SpinBot API pose a serious threat to academic integrity. It is extremely easy to copy an original paragraph and run it through a paraphrasing API to circumvent conventional plagiarism checkers. Methods have been explored to automatically classify machine-paraphrased content from human-generated content. These methods usually focus on using the entire paragraph to classify its originality. In this paper, we demonstrate it is possible to classify the content using just the first few sentences of the paragraph using BERT-based sentence embeddings. Additionally, we also explore the performance of MPNET sentence embeddings on this classification task.

Please refer to the "Final Report.pdf" file for a short paper on our project.

The dataset is split across the "dataset.zip.001" and "dataset.zip.002" files.

The "Dataset_preprocessor.ipynb" file generates sentence embeddings for the training and test sets. These sentence embeddings are stored as pkl files for conveniently feeding into the classifier models.

The "Model_trainer.ipynb" file represents the neural networks actually performing the classification task - machine paraphrased content or not. The pkl files representing the concatenated sentence embeddings of the paragraphs from the dataset are fed into this model.
