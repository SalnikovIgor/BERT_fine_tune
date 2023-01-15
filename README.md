Repository contains jupyter notebooks for fine tune and inference `bert-base-multilingual-uncased` model. 

## Dataset
To tune the model was used dataset: [Link](https://www.kaggle.com/datasets/aybatov/toxic-russian-comments-from-pikabu-and-2ch)

## Fine tune
To fine-tune the model, run the `finetune_bert` notebook and set the `DATA` variables, which specifies 
the path to your dataset, and `MODEL` which specifies which model you want to use as the base

## Model
The resulting model: [Link](https://drive.google.com/file/d/10NJzeGD8H60w94zq07jTmHd1lAlqBNAi/view?usp=share_link)

## Metrics
These results are obtained for the model `bert-base-multilingual-uncased` and dataset above

|              | precision | recall | f1-score | support |
|-------------:|----------:|-------:|---------:|--------:|
|            0 |      0.93 |   0.94 |     0.94 |    1934 |
|            1 |      0.88 |   0.86 |     0.87 |     949 |
|     accuracy |           |        |     0.92 |    2883 |
|    macro avg |      0.91 |   0.90 |     0.90 |    2883 |
| weighted avg |      0.91 |   0.92 |     0.91 |    2883 |

## Inference
To inference the model, run the `inference` notebook and set the variables:  
`MODEL`: name of base model  
`MODEL_FILE`: path to fine tune model  
`text`: input text



