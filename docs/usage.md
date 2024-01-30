# Models

## Setup

### Install requirements

```sh
pip install datasets
pip install transformers
pip install span-marker
```

### Usage

Models can be loaded from the HuggingFace Hub according to their name:

- iahlt/xlm-roberta-base-ar-ner-mafat-fold1
- iahlt/xlm-roberta-base-ar-ner-mafat-fold2
- iahlt/xlm-roberta-base-ar-ner-mafat-fold3
- iahlt/xlm-roberta-base-ar-ner-mafat-fold4
- iahlt/xlm-roberta-base-ar-ner-mafat (trained on 90%/10% train/validation split)

But before you can load the model, you need to login to the HuggingFace API using [the given token](access.md):

```sh
huggingface-cli login # insert your token when prompted
```

Then you can load the model and use it as follows:

```py
from span_marker import SpanMarker

model = SpanMarker.from_pretrained("iahlt/xlm-roberta-base-ar-ner-mafat")
```

A model can be used to predict spans in a text and return a list of char-based spans:

```py
text = """
يعيش 1.98 مليون رجل وامرأة في إسرائيل تحت خط الفقر، من بينهم 873.3 ألف طفل، 152.5 ألف مواطن مسن و949.6 ألف في سن العمل – هذا بحسب تقرير الفقر لعام 2022 الصادر عن مؤسسة التأمين الوطني والذي صدر يوم الخميس (28/12) وبحسب التقرير، يبلغ معدل الفقر بين عامة السكان 20.2%، دون تغيير عن عام 2021.
""".strip()  # https://ar.davar1.co.il/479583/
spans = model.predict(text)
print(spans)
# [{'span': ['إسرائيل'],
#   'label': 'GPE',
#   'score': 0.9982821941375732,
#   'word_start_index': 6,
#   'word_end_index': 7},
#  {'span': ['لعام', '2022'],
#   'label': 'TIMEX',
#   'score': 0.9435986280441284,
#   'word_start_index': 29,
#   'word_end_index': 31},
#  {'span': ['مؤسسة', 'التأمين', 'الوطني'],
#   'label': 'ORG',
#   'score': 0.967919647693634,
#   'word_start_index': 33,
#   'word_end_index': 36},
#  {'span': ['يوم', 'الخميس'],
#   'label': 'TIMEX',
#   'score': 0.9344639182090759,
#   'word_start_index': 38,
#   'word_end_index': 40},
#  {'span': ['عام', '2021.'],
#   'label': 'TIMEX',
#   'score': 0.9829164147377014,
#   'word_start_index': 53,
#   'word_end_index': 55}]
```

A model can be used to predict spans over a pre-tokenized text (returns a list of token-based spans):

```py
segmented_text = text.split()  # your tokenization/segmentation of text
print(model.predict(segmented_text))
# [{'span': ['إسرائيل'], 'label': 'GPE', 'score': 0.9982821941375732, 'word_start_index': 6, 'word_end_index': 7}, {'span': ['لعام', '2022'], 'label': 'TIMEX', 'score': 0.9435986280441284, 'word_start_index': 29, 'word_end_index': 31}, {'span': ['مؤسسة', 'التأمين', 'الوطني'], 'label': 'ORG', 'score': 0.967919647693634, 'word_start_index': 33, 'word_end_index': 36}, {'span': ['يوم', 'الخميس'], 'label': 'TIMEX', 'score': 0.9344639182090759, 'word_start_index': 38, 'word_end_index': 40}, {'span': ['عام', '2021.'], 'label': 'TIMEX', 'score': 0.9829164147377014, 'word_start_index': 53, 'word_end_index': 55}]
```

## Usage with spacy (optional)

It's possible to use the model with spacy, to do so, you need to install spacy and spacy-transformers
and stanza for Arabic (multiword tokenization) MWT(segmentation)

### Install requirements

```sh
pip install spacy
pip install spacy-transformers
pip install stanza spacy_stanza
```

```py
import spacy
import stanza
import spacy_stanza
from huggingface_hub import hf_hub_download

stanza.download("ar")
nlp = spacy_stanza.load_pipeline("ar", processors="tokenize,pos,lemma,depparse")
nlp.add_pipe("span_marker", config={"model": "iahlt/xlm-roberta-base-ar-ner-mafat"})
```

And then you can use the model with spacy as usual:

```py
doc = nlp(text)

for ent in doc.ents:
    print(ent.text, ent.start_char, ent.end_char, ent.label_)
# إسرائيل 31 38 GPE
# عام 2022 150 158 TIMEX
# مؤسسة التأمين الوطني 169 189 ORG
# يوم الخميس 201 211 TIMEX
# 28 / 12 ) 214 223 TIMEX
# عام 2021 . 296 306 TIMEX
```

visualize the entities:

```py
from spacy import displacy

displacy.render(doc, style="ent", jupyter=True)
```
 
