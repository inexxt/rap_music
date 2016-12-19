# Analysis of polish rap music

---

## Project description

Rap jest powszechnie uważany za jedną z mniej ambitnych form muzyki. Prostackie teksty skoncetrowane na przemocy, narkotykach i zarabianiu pieniędzy, prosty bit, powtarzające się motywy, wulgaryzmy pojawiające się w co drugim wersie. 
Sam będąc fanem rapu, widzę ten gatunek zupełnie inaczej. Moim zdaniem negatywna opinia jest oparta na stereotypie. Widzę tę muzykę przez pryzmat niezwykłej elokwencji i mistrzostwa w operowaniu językiem. Postanowiłem więc zebrać wszystkie dostępne mi teksty, przeanalizować je i porównać raperów (i nieraperów) pod względem zasobu słownictwa, użycia wulgaryzmów, popularności etc.

Notebooki w tym repozytorium powinno uruchamiać się po kolei, w każdym z nich ustawiając w nagłówku ścieżkę do folderu, w którym mają być zapisywane teksty etc. Do poprawnego działania jest też potrzebny polski słownik morfosyntaktyczny, który można znaleźć pod adresem (TODO). W projekcie nie używam nltk ani żadnego innego gotowego narzędzia, bo nie mają wsparcia dla języka polskiego, i dlatego potrzebne są dodatkowe zależności.

## Notebooks description

Notebooki robią następujące rzeczy:

0. Ściągnięcie listy raperów (opierając się na liście raperów, którzy wzięli udział w Hot16 - (link)), scrawlowanie ich tekstów z rapgeniusa, wyczyszczenie części tekstów (tylko pod względem języka (oddzielenie polskiego od angielskiego), przypisania autorstwa itp).
1. Preprocessing tekstów - czyszczenie, stemming, oraz przygotowanie słowników.
2. Analiza wulgaryzmów, elokwencji, popularności, słownictwa.
3. Użycie Doc2vec do stworzenia wektorów raperów, klastrowanie ich z użyciem **Affinity propagation**  i **Spectral clustering**, wizualizacja za pomocą **PCA** i **t-SNE**.
4. Użycie R-owego ggplot2 do wygenerowania 2-wymiarowego wykresu.


## TODO:

Do zrobienia jest jeszcze dorzucenie klasycznej polskiej literatury i poezji.

## Requirements

* python 3.5
* gensim
* numpy
* sklearn
* pandas
* tqdm
* langdetect
* seaborn
* matplotlib