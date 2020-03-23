# Auto-Generate-Text-Based-Answers
##### Generate upto 3 distractors for each Question-Answer combination

## About Problem Statement:
1. Genre: NLP
2. Problem Type: Contextual Semantic Similarity, Auto generate Text-based answers

## Submission Format:

1. You need to generate upto 3 distractors for each Question-Answer combination
2. Each distractor is a string
3. The 3 distractors/strings need to be separated with a comma (,)
4. Each value in Results.csv's distractor column will contain the distractors as follows: distractor_for_QnA_1 = "distractor1","distractor2","distractor3"

## About the Evaluation Parameter:

1. All distractor values for 1 question-answer will be converted into a vector form
2. 1 vector gets generated for submitted distractors and 1 vector is generated for truth value
cosine_similarity between these 2 vectors is evaluated
3. Similarly, cosine_similarity gets evaluated for all the question-answer combinations
4. Score of your submitted prediction file = mean ( cosine_similarity between distractor vectors for each entry in test.csv)
