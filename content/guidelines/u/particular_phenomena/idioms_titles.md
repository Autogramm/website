---
layout: default
---
# Idioms and titles



In SUD we decided to call this phenomena idioms and not MWEs because we consider that MWE is a larger term as they englobe named entities as well. 

Theoretical background: what is an idiom and how to distinguish it
…
…
...
Why we won’t be using the fixed relation:
The property of being fixed is a property of the whole expression and not of each relation individually. This expression may contain more than two relations. Therefore, there is no more reason to mark relations than tokens.
The label fixed is already used in UD with more restrictions, especially with only continuous MWEs.
Implementation: The arguments above are why we decided to annotate this information within the nodes and not within the syntactic relations.
Practical overview
The head of an idiom / title has a ExtPos feature that indicates the POS of the chunk within the sentence
ex : I like the movie One Flew Over The Cuckoo's Nest. 
As this is a title, its head will have an ExtPos=PROPN
NOTE: all titles have the same ExtPos ; PROPN
The head of an idiom / title will also have a feature PhraseType=Title or PhraseType=Idiom
Each component of an idiom / title will have a respective feature InIdiom=Yes or InTitle=Yes
+ Example of an idiom