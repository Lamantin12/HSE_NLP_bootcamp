## Classes
1) class Vocabulary:  

    **Variables**
    * token_to_idx
    * idx_to_token
    
    **Methods**
    * \_\_init__
    * add_token
    * lookup_token
    * lookup_index
    * \_\_len__


2) class SequenceVocabulary(Vocabulary):

    **Variables**
    * _mask_token
    * _unk_token
    * _begin_seq_token ***optional***
    * _end_seq_token ***optional***
    * mask_index
    * unk_index
    * begin_seq_index ***optional***
    * end_seq_index ***optional***

    **Methods**
    * \_\_init__
    * lookup_token

3) class Vectorizer:

    **Variables**
    * vocabulary

    **Methods**
    * \_\_init__
    * vectorize
    * from_dataframe

4) class JobsDataset(torch.utils.data.Dataset)
  
    **Variables**

    **Methods**
   * \_\_init__
   * \_\_getitem__
   * \_\_len__
   * get_num_batches
   * load_dataset_and_make_vectorizer


## TODO
* **Attention**
  max_sequence_length may not be same for datasets
* For preprocessing:
  1) Delete punctuation signs
  2) Try with/without stemming(don't like it)
  3) Try lemmatization ***optional***
* For models:  
  1) Try predicting logarythms
  2) Try pretrained embeddings
 
* For beauty:  
  1) Put all classes as well as functions in helper.py


## Ideas:
1) Try Conv text, then concat with other data and few linears then
2) Try w2v key_skills, kluster them and divide
3) Create json of translated sentences to vectors