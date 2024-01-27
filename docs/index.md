# Dataset

This is the documentation for IAHLT Arabic NER corpus and models.

## Corpus

### Schema and entity types
The corpus was annotated by IAHLT team. It contains 40,000 samples annotated with BILOU scheme as follows:    
    `B-` - the first token of a multi-token entity    
    `I-` - an inner token of a multi-token entity    
    `L-` - the last token of a multi-token entity    
    `U-` - a single-token entity (unit entity)     
    `O` - a non-entity token    
 
And the following entity types:    
`ANG` - Any named language (Hebrew, Arabic, English, French, etc.)      
`DUC` - A branded product, objects, vehicles, medicines, foods, etc. (Apple, BMW, Coca-Cola, etc.)     
`EVE` - Any named event (Olympics, World Cup, etc.)     
`FAC` - Any named facility, building, airport, etc. (Eiffel Tower, Ben Gurion Airport, etc.)     
`GPE` - Geo-political entity, nation states, counties, cities, etc.     
`INFORMAL` - Informal language (slang)     
`LOC` - Non-GPE locations, geographical regions, mountain ranges, bodies of water, etc.     
`ORG` - Companies, agencies, institutions, political parties, etc.     
`PER` - People, including fictional.     
`TIMEX` - Time expression, absolute or relative dates or periods.     
`TTL` - Any named title, position, profession, etc. (President, Prime Minister, etc.)     
`WOA` - Any named work of art (books, movies, songs, etc.)     
`MISC` - Miscellaneous entities, that do not belong to the previous categories     
      
### Statistics

| entity_tag | count   |
| ---------- | ------- |
| O          | 1419405 |
| PER        | 68167   |
| ORG        | 61642   |
| GPE        | 56185   |
| TIMEX      | 27759   |
| MISC       | 22461   |
| TTL        | 21765   |
| LOC        | 13905   |
| FAC        | 13658   |
| WOA        | 9353    |
| EVE        | 8427    |
| DUC        | 5368    |
| ANG        | 1964    |
| INFORMAL   | 91      |

### Links            
          

The corpus is available in the following formats:

* [Corpus](https://huggingface.co/datasets/iahlt/arabic_ner_mafat) - the original corpus 
* [Folds](https://huggingface.co/datasets/iahlt/arabic_ner_mafat_folds) - the corpus split into 4 folds for cross-validation

### Fields

Each sample contains the following fields:

* `id` - the sample id
* `tokens` - the list of tokens
* `ner_tags` - the encoded list of NER tags in BILOU scheme
* `raw_tags` - the list of NER tags in BILOU scheme


### Dataset loading

Need to install the `datasets` library:

```bash
pip install datasets
```
and login to the HuggingFace API using the given token:

```bash
huggingface-cli login # insert your token when prompted
```

Then you can load the corpus as follows:
    
```py
from datasets import load_dataset

dataset = load_dataset("iahlt/arabic_ner_mafat", split="train") # it has all the data in one split
for sample in dataset:
    print(sample)
```

```py
from datasets import load_dataset

folds_dataset = {}

for fold in ["fold_1", "fold_2", "fold_3", "fold_4"]:
    folds_dataset[fold] = load_dataset("iahlt/arabic_ner_mafat_folds", fold)

```

