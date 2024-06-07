# Textual-Emotion-Cause-Pair-Extraction-in-Conversations

# Task and dataset:
This is a SemEval 2024 task-3 (subtask 1) that focused on creating a model that could extract the emotion-cause pair from a conversation.
Our task was to predict the emotion for the given dialogue and give the appropriate cause for the emotion from the given conversation. 

For this task, the dataset was provided to us by SemEval which was a JSON file of a conversation list from the sitcom "FRIENDS".

# Dependencies:
- python 3.11.0
- Tensorflow 1.15.4
- RoBERTa pre-trained model
- Logistic regression model


# Basic Information about the project:
for this task, we have used 2 different models for predicting the emotion and fetching the cause for this emotion from the given conversation data.
for predicting the emotion for this task we used a Logistic Regression model. 
To get the Cause for the emotion we treated this problem as a question-answer approach and used a pre-trained RoBERTa model, i.e. the emotion predicted by the LR model was taken as a question for the RoBERTa model, and the context part we used the text data from all the conversation. So what this model did was search for the ans that is the cause from the context and give it as an output.

# Project Architecture:

<img width="968" alt="Screenshot 2024-06-07 at 12 14 07 AM" src="https://github.com/Shruti2301/Textual-Emotion-Cause-Pair-Extraction-in-Conversations/assets/71042986/16426e98-717c-49fe-bd12-b0c8f41f815f">


# CITATION

@ARTICLE{wang2023multimodal,
  author={Wang, Fanfan and Ding, Zixiang and Xia, Rui and Li, Zhaoyu and Yu, Jianfei},
  journal={IEEE Transactions on Affective Computing}, 
  title={Multimodal Emotion-Cause Pair Extraction in Conversations}, 
  year={2023},
  volume={14},
  number={3},
  pages={1832-1844},
  doi = {10.1109/TAFFC.2022.3226559}
}

@InProceedings{wang2024SemEval,
  author={Wang, Fanfan  and  Ma, Heqing  and  Xia, Rui  and  Yu, Jianfei  and  Cambria, Erik},
  title={SemEval-2024 Task 3: Multimodal Emotion Cause Analysis in Conversations},
  booktitle={Proceedings of the 18th International Workshop on Semantic Evaluation (SemEval-2024)},
  month={June},
  year={2024},
  address={Mexico City, Mexico},
  publisher={Association for Computational Linguistics},
  pages={2022--2033},
  url = {https://aclanthology.org/2024.semeval2024-1.273}
}
