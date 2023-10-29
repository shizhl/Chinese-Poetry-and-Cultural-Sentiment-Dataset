# Chinese-Poetry-and-Cultural-Sentiment-Dataset
The dataset for Chinese Poetry and Cultural Sentiment.
## Content

- [How We Made this Dataset](#how-we-made-this-dataset)
- [How To Use this Dataset](#how-to-use-this-dataset)
- [Project We Reference](#project-we-reference)



## How We Made this Dataset
Since there are currently very few sculptures from the Wei, Jin, Southern and Northern Dynasties, and Sui Dynasties in museums in China, the data obtained from the official websites of each museum cannot meet our needs. Therefore, we first crawled data from the museum's website, and then this part of the data is used as a query, and wiki is used to perform related searches, and chatgpt is used to organize the search results to generate text data that can be used. We use the text compiled by chatgpt as input, and let chatgpt retrieve this part of the text again and output it. The name of a sculpture contemporaneous with the artifact described in this section of text. We used the output name as query for iterative search, and finally obtained this dataset.
## How To Use this Dataset
We saved the obtained dataset in the folder 'dataset', file 'data.json'. Each element in this file stores data from a sculpture artifact, where 'id' is the number we gave when making the dataset, and 'title' is the name of this cultural relic, and 'text' is the description of this cultural relic.
<br>
Since the iterative search answers of chatgpt are not controllable when making the data set, there is some duplicate data in this data set, as well as some data that does not describe sculpture cultural relics.
## Project We Reference
Regarding Tang poetry and Song lyrics, we used the data set produced by the GitHub project [chinese-poetry](https://github.com/chinese-poetry/chinese-poetry)<br>
We hereby express our thanks.
