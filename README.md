# AWS NLP Summit 2022 Hands-on Workshop
AWS NLP Summit 2022 - Hands-on Workshop W07 Hugging Face Model Explainability for customer sentiment text analytics using SageMaker Clarify
https://www.aws-nlp-summit.com/

In the workshop, we will use Amazon Review data set from Kaggle to train Hugging face mode, and predict customer sentiments, after use Amazon SageMaker Clarify to explain the hugging face models, which can help you understand which sections of text are most important for the predictions made by your model. This functionality can be used to explain an individual local prediction. You can define the length of the text segment (tokens, phrases, sentences, paragraphs) to understand and visualize a model’s behavior at multiple levels of granularity.

Traning and test dataset from Kaggle https://www.kaggle.com/datasets/bittlingmayer/amazonreviews

Pre-requirments.

1. Sign-in Kaggle account,
2. Download new API Token file (kaggle.json) in your local, and upload into your notebook.Please refer the doc. https://github.com/Kaggle/kaggle-api


The notebook will first train a Hugging Face model using the Hugging Face Estimator in the SageMaker Python SDK using training dataset, then use SageMaker Clarify to analyze a testing dataset in CSV format, and then visualize the results.

For Hugging face model training and endpoint, it need AWS SageMaker GPU instacnes. E.g. for training, ml.p3.2xlarge, for endpoint ml.g4dn.xlarge
