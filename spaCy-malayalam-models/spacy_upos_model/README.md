# Usage


## Installation
Install from spaCy github repository until they officially release the Malayalam Language class.
```
pip install git+https://github.com/explosion/spaCy.git

```

## Execution
```
import spacy
model = spacy.load("./")
sentence = "ചെങ്ങന്നൂര്‍ : വെള്ളപ്പൊക്കത്തെ അതിജീവിച്ച് പിടിച്ചുനിന്ന കരിമ്പും ഒടുവില്‍ കീഴടങ്ങുന്നു ."
doc = model(sentence)
for item in doc:
    print(item.text, item.tag_)
```

## Sample Result
```
ചെങ്ങന്നൂര്‍ PROPN
: PUNCT
വെള്ളപ്പൊക്കത്തെ NOUN
അതിജീവിച്ച് VERB
പിടിച്ചുനിന്ന VERB
കരിമ്പും NOUN
ഒടുവില്‍ ADV
കീഴടങ്ങുന്നു VERB
. PUNCT
```
