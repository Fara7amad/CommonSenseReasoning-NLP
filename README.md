# CommonSenseReasoning-NLP
Assignment for the NLP course at An-Najah National University
---

1. Objective:
      - To build a system that can outperform a baseline model with an accuracy of 0.2 using fastText, word2vec, and GloVe word embeddings.
      - Additionally, compare the performance of these pretrained embedding models in terms of accuracy.

   
2. Task Description:
      - You are provided with a file containing a number of multiple-choice questions (MCQs), where each question has the correct answer. The questions are related to common sense reasoning.
      - Data Format: Each question in the file is represented as a JSON object with the following format:
```json
{
  "answerKey": "A",
  "id": "075e483d21c29a511267ef62bedc0461",
  "question": {
    "question_concept": "punishing",
    "choices": [
      {
        "label": "A",
        "text": "ignore"
      },
      {
        "label": "B",
        "text": "enforce"
      },
      {
        "label": "C",
        "text": "authoritarian"
      },
      {
        "label": "D",
        "text": "yell at"
      },
      {
        "label": "E",
        "text": "avoid"
      }
    ],
    "stem": "The sanctions against the school were a punishing blow, and they seemed to what the efforts the school had made to change?"
  }
}
```
3. Requirements:
      - Use fastText, word2vec, and GloVe word embeddings to build a system for common sense reasoning.
      - No need to learn the word embeddings.
      - You can download and utilize them in the task.
      - Note that you can use gensim library in python to download and look-up word embeddings
        
      ```python
      import gensim
      
      # Load pre-trained Word2Vec model.
      
      model = gensim.models.Word2Vec.load("modelName.model")
      ```


    - Evaluate your model's performance and ensure it outperforms a baseline model with an accuracy of 0.2.
    - Compare the performance of your model using different word embeddings.

      
4. Evaluation Criteria:
      - Accuracy of the model in outperforming the baseline (minimum 0.2 higher accuracy).
      - Clarity and conciseness of the code.
