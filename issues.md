# Issues

## Words
- Should gender be a field?
- Should singular/plural be a field?
- Should "Examples" in the Words table link to records in the Sentences table?


## Sentences
- Should records with all three of a Dialectal, MSA, and English translation be converted into one-to-one relationships linked by a common ID#? Because right now they are three-way translations.
- Big Question: Should words (of any type) be linked to Sentences through Examples?


## Bigger-Picture Database Architecture?
- It seems clear that *Verbs* (and quite likely that also *Verb Conjugations*) should be stored in a separate table. What about *Words*? Currently, Words are stored in a single table, with the _Part of Speech_ field being the indicator of differentiation. Should these instead be on a separate table?
- How to structure translations of sentences? Should every record have an "English" field plus a dialectal Arabic field? Or will these need to be related to another linked table? 


## Verbs
- Which format/schema of conjugation should be used? (See examples)
- Should verbs and conjugations be separate tables? 
 - Same table: using 'conjugation' field to denote tense/person etc
 - Different tables: One table for roots, another for conjugations same as above
- How to append notes on word definitions, for example alternative meanings or 'literal' meaning? Ex.: "خِلِق" - to be born, ++ literally, to be created
- How to add verb form features? As play text, or as linked options list?




