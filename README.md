# Analysis of polish rap music

### Project description

Rap is commonly considered as one of the less sophisicated genres of music. Coarse lyrics focusing mainly on agression, drugs and money, oversimplified beat, repetitive themes, widespread strong language usage.

I, being a rap music enthusiast myself, see that genre in quite different way. In my opinion the negative opinion is based on stereotypes, which are based on both historical contexts and most popular artist work, which aren't representative for the genre.

I see the music through the lenses of unbelievable eloquence, the mastery of language itself, intuitions about the words and rhytm. That's why I decided to collect all the lyrics I could have get my hands on then clean, process and analyze them, and compare rappers and some non-rappers widely accepted as great writers in terms of vocabulary richness, strong language usage, popularity, etc.

### Instruction

Names of the notebooks in this repository reflect the order in which they should be run. Each of them require setting of path variables at the beginning, which should be consistent between them. 

To run, you also need Polimorfologik: a polish morphosyntactic dictionary, which can be found here: https://github.com/morfologik/polimorfologik/releases/tag/2.1

NLTK nor any different language library is used in the project, since none of them supports polish.

### What is actually happening here 

Notebooks are doing following things:

- Downloading a list of polish rappers (based on the list of rappers that took part in the Hot16 - a facebook-chain-challenge) from rapgenius, then downloading their lyrics, pre-cleaning them (attributing to the correct artist, language detection, etc.)
- Preprocessing of lyrics - cleaning, stemming, preparation of the dictionaries.
- Analysis of strong language, popularity and vocabulary.
- Doc2rapper :) adaptation of Doc2vec, with experiments on simarity, using Spectral clustering and Affinity propagation, visualizations using PCA and t-SNE.
- R based notebook for better visualization.

### Todo

For now, there are only rappers analyzed, in the future it should also include poets and writers.

### Requirements

- python 3.5
- gensim 0.13
- numpy 1.12
- scikit-learn 0.18
- pandas 0.18
- tqdm
- langdetect
- seaborn
- matplotlib
