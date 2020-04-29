# Usage

```
import spacy
model = spacy.load("./")
sentence = "ചെങ്ങന്നൂര്‍ : വെള്ളപ്പൊക്കത്തെ അതിജീവിച്ച് പിടിച്ചുനിന്ന കരിമ്പും ഒടുവില്‍ കീഴടങ്ങുന്നു ."
doc = model(doc)
for item in doc:
    print(item.text, item.tag_)
```
