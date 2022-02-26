# Turkish_Bert_Question_Answering_Fine-Tuning
You can fine-tune your question answering model with your own dataset with this repo.

[You can find the model trained with this notebook in huggingface.](https://huggingface.co/oguzhanolm/loodos-bert-base-uncased-QA-fine-tuned)

---
language: tr
tags:
- question-answering
- loodos-bert-base
- TQuAD 
- tr
datasets:
- TQuAD
model-index:
- name: loodos-bert-base-uncased-QA-fine-tuned
  results: 
  - task:
      name: Question Answering
      type: question-answering
    dataset:
      name: TQuAD
      type: question-answering
      args: tr
    metrics:
      - name: Accuracy 
        type: acc
        value: 0.91
---

# Turkish SQuAD  Model : Question Answering

I fine-tuned Loodos-Turkish-Bert-Model for Question-Answering problem with TQuAD dataset. Since the "loodos/bert-base-turkish-uncased" model gave the best results for the Turkish language in classification in the "Auto-tagging of Short Conversational Sentences using Transformer Methods" research we conducted with my teammates, I used this model because I thought that the success rate could be high in the question-answering.
* Loodos-BERT-base-uncased: https://huggingface.co/loodos/bert-base-turkish-uncased
* TQuAD dataset:  https://github.com/TQuad/turkish-nlp-qa-dataset
