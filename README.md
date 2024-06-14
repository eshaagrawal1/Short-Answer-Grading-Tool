# Short Answer Grading System
# Abstract
The Short Answer Grading System is an advanced platform designed to automatically grade responses. Using state-of-the-art performance, this system tackles one of the key challenges in Natural Language Processing (NLP) and educational assessment. It leverages a deep neural network framework based on the Bidirectional Encoder Representation from Transformers (BERT) to efficiently grade subjective answers, reducing the workload and costs for educational institutions. This project outlines the methodology, implementation, and performance of the system, demonstrating a scoring accuracy of 0.77 for binary grading and 0.57 for a 0-5 score range.

#  Introduction
Evaluating student knowledge is crucial for effective teaching, and while multiple choice questions (MCQs) are easier to grade, subjective questions like short answers or essays are more challenging. The ASAG system proposed here uses a BERT-based deep neural network framework to automate the grading process. This reduces the manual effort required for grading, making the process more efficient and cost-effective.

# Related Work
Recent studies have explored various approaches for automatic short answer grading using machine learning and NLP techniques. The BERT model has emerged as a powerful tool, achieving high accuracy in several tasks. Previous works have focused on using different models like LSTM, CNN, and traditional machine learning techniques, each contributing to the advancement of ASAG systems.

# Methodology
Datasets
The SciEntsBank (SEB) dataset was used for this study, containing science assessment questions and student responses. The dataset includes labels indicating whether each response is correct or incorrect.

![Screenshot 2024-06-14 234947](https://github.com/eshaagrawal1/Short-Answer-Grading-Tool/assets/90109712/a3c63d19-0e41-40d3-ba41-a7b52ef1bacb)


# Data Pre-Processing
The dataset underwent preprocessing to enhance its quality for model training. This included tokenization, stemming, lemmatization, and computing cosine similarity scores.

# Model Assumption
The BERT model, pre-trained on English Wikipedia and fine-tuned on the SEB dataset, was used for grading. Each (question, reference answer, student answer) triplet was processed to generate a similarity score.

![Screenshot 2024-06-14 235026](https://github.com/eshaagrawal1/Short-Answer-Grading-Tool/assets/90109712/b34a9df1-574a-48f8-8512-924c3ce183be)

# Model Translation
TensorFlow's implementation of Light-BERT was leveraged for this project. The fine-tuned BERT model was used to predict scores for student responses.

![Screenshot 2024-06-14 235256](https://github.com/eshaagrawal1/Short-Answer-Grading-Tool/assets/90109712/6f5d9c68-8ad0-41cf-a8ce-ced379247d39)

# Results
The system demonstrated an accuracy of 0.77 for binary scoring (correct/incorrect) and 0.57 for scoring on a range of 0-5. The binary scoring system proved to be more accurate.

![Screenshot 2024-06-14 235050](https://github.com/eshaagrawal1/Short-Answer-Grading-Tool/assets/90109712/ce7f918f-e7ce-494c-970d-babe7f6dc811)
![Screenshot 2024-06-14 235142](https://github.com/eshaagrawal1/Short-Answer-Grading-Tool/assets/90109712/5601035a-d978-48e2-8144-c8360095ca63)
![Screenshot 2024-06![Screenshot 2024-06-14 235234](https://github.com/eshaagrawal1/Short-Answer-Grading-Tool/assets/90109712/ab0ed14a-902d-4de2-b7d1-f04c9d7396ea)
-14 235212](https://github.com/eshaagrawal1/Short-Answer-Grading-Tool/assets/90109712/63f6f97f-faba-49f5-86db-e718197472eb)
![Screenshot 2024-06-14 235450](https://github.com/eshaagrawal1/Short-Answer-Grading-Tool/assets/90109712/5be3e28a-e012-47bf-8bd7-b269a1ae20e3)




