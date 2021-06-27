# Unintended-Bias-Toxicity-Detection-Project

## Description

This project dataset hasbeen collected from a previously ended Kaggle Competition named [Jigsaw Unintended Bias in Toxicity Classification](https://www.kaggle.com/c/jigsaw-unintended-bias-in-toxicity-classification/data) where the task was to detect toxicity across a diverge range of conversations.

### File descriptions
* train.csv - the training set, which includes toxicity labels and subgroups
* test.csv - the test set, which does not include toxicity labels or subgroups
* sample_submission.csv - a sample submission file in the correct format

* test_public_expanded.csv - The public leaderboard test set, including toxicity labels and subgroups. The competition target was a binarized version of the toxicity column, which can be easily reconstructed using a >=0.5 threshold.
* test_private_expanded.csv - The private leaderboard test set, including toxicity labels and subgroups. The competition target was a binarized version of the toxicity column, which can be easily reconstructed using a >=0.5 threshold.
* toxicity_individual_annotations.csv - The individual rater decisions for toxicity questions. Columns are:<br>
*id - The comment id. Corresponds to id field in train.csv, test_public_labeled.csv, or test_private_labeled.csv.
worker - The id of the individual annotator. These worker ids are shared between toxicity_individual_annotations.csv and identity_individual_annotations.csv.<br>
toxic - 1 if the worker said the comment was toxic, 0 otherwise.<br>
severe_toxic - 1 if the worker said the comment was severely toxic, 0 otherwise. Note that any comment that was considered severely toxic was also considered toxic.<br>
identity_attack, insult, obscene, sexual_explicit, threat - Toxicity subtype attributes. 1 if the worker said the comment exhibited each of these traits, 0 otherwise.<br>*
* identity_individual_annoations.csv - The individual rater decisions for identity questions. Columns are:<br>
*id - The comment id. Corresponds to id field in train.csv, test_public_labeled.csv, or test_private_labeled.csv.<br>
worker - The id of the individual annotator. These worker ids are shared between toxicity_individual_annotations.csv and toxicity_individual_annotations.csv.<br>
disability, gender, race_or_ethnicity, religion, sexual_orientation - The list of identities within this category that the rater noticed in the comment. Formatted a space-separated strings.<br>*

### Dependencies

* Python 3, NumPy, Pandsas, PyTorch, Pretrained (BERT, GPT2, XLNet) models
* Kaggle environment (recommended)

### Installing and Executing Program

* Download the main .ipynb file
* To run this project on your local machine, you need to download [BERT large and small, GPT2, XLNet Models](https://www.kaggle.com/haqishen/jigsawmodels) and [Pytorch Pretrained BERT model](https://www.kaggle.com/haqishen/pytorchpretrainedberthaqishen) manually
* To run on kaggle environment, just make sure that you add these saved and pretrained models as input data


## Help

If you face any problem to run this notebook, make sure that you have turned on GPU because this script won't run on CPU runtime. If you encounter error while submitting the predictions on Kaggle, before submission you've to run the entire notebook keeping the 'Internet mode' off on Kaggle kernel.

## Authors

[Md. Abrar Jahin](https://www.linkedin.com/in/md-abrar-jahin-9a026018b/)

## License

This project is licensed under the [Apache License 2.0] License - see the LICENSE.md file for details

## Acknowledgments

Inspiration, code snippets, etc.
* [How To: Preprocessing for GloVe Part2: Usage](https://www.kaggle.com/christofhenkel/how-to-preprocessing-for-glove-part2-usage)
* [How To: Preprocessing for GloVe Part1: EDA](https://www.kaggle.com/christofhenkel/how-to-preprocessing-for-glove-part1-eda)
