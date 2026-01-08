# Fine-tuning of distilBERT for Named Entity Recognition

Fine-tuning of a pre-trained model for named entity recognition in English.

Files :
* model_fine_tuning_NER.ipynb : data processing and fine-tuning of the model
* correction_annotation - corpus_anno_no_text.csv : training data

The data comes from news articles written in English and published in October 2025. The articles were downloaded from the Europresse platform.

The articles were first annotated using the ```english_web_core_trf``` spaCy pipeline. The annotations were then corrected by 4 annotators, and exported in a .csv file to be used as data to fine-tune the model.

Pre-trained model that was fine-tuned : https://huggingface.co/distilbert/distilbert-base-uncased 

The model is then evaluated using a confusion matrix. The results are very encouraging.
<br></br>
*Please note that much of the code used here is either inspired by or directly taken from Ms. Delphine Bernhard's Machine Learning course given at the Université de Strasbourg.*
