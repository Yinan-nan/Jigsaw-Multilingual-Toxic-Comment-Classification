# Jigsaw-Multilingual-Toxic-Comment-Classification
(Use TPUs to identify toxicity comments across multiple languages)

# Problem Description
It only takes one toxic comment to sour an online discussion. The Conversation AI team, a research initiative founded by Jigsaw and Google, builds technology
to protect voices in conversation. A main area of focus is machine learning models that can identify toxicity in online conversations, where toxicity is defined 
as anything rude, disrespectful or otherwise likely to make someone leave a discussion. If these toxic contributions can be identified, we could have a safer, 
more collaborative internet.

In the previous 2018 Toxic Comment Classification Challenge, Kagglers built multi-headed models to recognize toxicity and several subtypes of toxicity.
In 2019, in the Unintended Bias in Toxicity Classification Challenge, you worked to build toxicity models that operate fairly across a diverse range of 
conversations. This year, we're taking advantage of Kaggle's new TPU support and challenging you to build multilingual models with English-only training data.

Jigsaw's API, Perspective, serves toxicity models and others in a growing set of languages (see our documentation for the full list). Over the past year,
the field has seen impressive multilingual capabilities from the latest model innovations, including few- and zero-shot learning. We're excited to learn
whether these results "translate" (pun intended!) to toxicity classification. Your training data will be the English data provided for our previous two 
competitions and your test data will be Wikipedia talk page comments in several different languages.

As our computing resources and modeling capabilities grow, so does our potential to support healthy conversations across the globe. Develop strategies to
build effective multilingual models and you'll help Conversation AI and the entire industry realize that potential.

# Data collected from kaggle
The primary data for the competition is, in each provided file, the comment_text column. This contains the text of a comment which has been classified as toxic 
or non-toxic (0...1 in the toxic column). The train set’s comments are entirely in english and come either from Civil Comments or Wikipedia talk page edits.
The test data's comment_text columns are composed of multiple non-English languages.

The *-train.csv files and validation.csv file also contain a toxic column that is the target to be trained on.

The jigsaw-toxic-comment-train.csv and jigsaw-unintended-bias-train.csv contain training data (comment_text and toxic) from the two previous Jigsaw competitions, 
as well as additional columns that you may find useful.

# Predicting
I am predicting the probability that a comment is toxic. A toxic comment would receive a 1.0. A benign, non-toxic comment would receive a 0.0. In the test set, 
all comments are classified as either a 1.0 or a 0.0
