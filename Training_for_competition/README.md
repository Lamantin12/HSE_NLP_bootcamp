## Classes
* class Vocabulary:
    * \_\_init__()
    * to_serializable()
    * from_serializable()
    * add_token
    * add_many
    * lookup_token
    * lookup_index
    * \_\_str__
    * \_\_len__

* class SequenceVocabulary(Vocabulary):
    * to_serializable
    * lookup_token

* class Vectorizer:
    * \_\_init__
    * vectorize
    * from_dataframe
    * from_serializable
    * to_serializable

* class JobsDataset(torch.utild.data.Dataset)
   * \_\_init__
   * \_\_getitem__
   * \_\_len__


## TODO:
* For preprocessing:
  1) Try with/without stemming(don't like it)
  2) Try lemmatization ***optional***
* For models:  
  1) Try predicting logarythms
  2) Try pretrained embeddings
  3) 