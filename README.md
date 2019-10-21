## Predicting Insincere Questions on Quora

This blog post is about the challenge that is hosted on kaggle [Quora Insincere Questions](https://www.kaggle.com/c/quora-insincere-questions-classification/overview). 

This post is divided into five parts:

1. Overview
2. Evaluation Metrics
3. Basic EDA and Data Preprocessing
4. Base Line Model
5. Deep Learning Models
6. Conclusion

Lets get started!

![GIF](https://media1.tenor.com/images/7dcc0b5a2c64d741b6edd12a88738cf9/tenor.gif?itemid=4767352)

### 1. Overview:
Quora is a platform that empowers people to learn from each other. One can go to Quora and ask their questions and get answers from others. But some questions asked by users may be toxic and contain divisive content. The aim of the competition is to tackle these situations.

The dataset is a csv file you can download it from [here](https://www.kaggle.com/c/quora-insincere-questions-classification/data).

<b>qid</b>: Question ID

<b>question_text</b>:  Question text.

<b>target</b>: target whether the question is sincere or not. if question is insincere then target is 1 else 0.


### 2. Evaluation Metrics
F1-Score = 2 x (precision x recall) / (precision + recall)

<b>Precision</b>: The precision is the ratio tp / (tp + fp) where tp is the number of true positives and fp the number of false positives. The precision is intuitively the ability of the classifier not to label as positive a sample that is negative.

<b>Recall</b>: The recall is the ratio tp / (tp + fn) where tp is the number of true positives and fn the number of false negatives. The recall is intuitively the ability of the classifier to find all the positive samples.

### 3. Basic EDA and Data Preprocessing
```python
# load the dataset
train_df = pd.read_csv('train.csv')
```


### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for
An existential problem for any major website today is how to handle toxic and divisive content
```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/suryachintu/Quora-Insincere-Questions-Kaggle/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
