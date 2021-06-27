# Unintended-Bias-Toxicity-Detection-Project

Simple overview of use/purpose.

## Description

This project dataset hasbeen collected from a previously ended Kaggle Competition named [Jigsaw Unintended Bias in Toxicity Classification](https://www.kaggle.com/c/jigsaw-unintended-bias-in-toxicity-classification/data) where the task was to detect toxicity across a diverge range of conversations.

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
