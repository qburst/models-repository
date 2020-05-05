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
ചെങ്ങന്നൂര്‍ N_NNP
: RD_PUNC
വെള്ളപ്പൊക്കത്തെ N_NN
അതിജീവിച്ച് V_VM_VNF
പിടിച്ചുനിന്ന V_VM_VNF
കരിമ്പും N_NN
ഒടുവില്‍ RB
കീഴടങ്ങുന്നു V_VM_VF
. RD_PUNC
```
