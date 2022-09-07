# BoE_ARP_insurance_risk_dection
The dissertation in collaboration with Bank of England to apply NLP to detect insurance firms risks

## Methodology
<img width="814" alt="image" src="https://user-images.githubusercontent.com/61338647/188922377-e82457e3-8582-455e-8408-75587d0dd7e0.png">

## DTM and LDA model
- "get_topic_dist": Retrieves all topics probabilities of the paragraph. Instead of giving the label of a specific topic, a single paragraph might describe multiple topics, and retrieving all topics' probabilities would help present more detailed and precise data.
- "get_topic_word": Generates the words by sorted probability of each topic, and it would give us a general topic concept when seeking business insights.
<img width="492" alt="image" src="https://user-images.githubusercontent.com/61338647/188922579-58288aa1-6a67-40e2-9a99-f97bc4c3f39a.png">

## Result of dynamic topic modelling (DTM) 
- Analyzed extreme probability values at specific time points.
- Early time (2011 to 2014), Middle time (2015 to 2018), Recent time (2019 to 2021)
![MD-DTM_1](https://user-images.githubusercontent.com/61338647/188923939-82c06a13-7349-42bd-97e2-4f012529521c.png)
![QA-DTM_1](https://user-images.githubusercontent.com/61338647/188924055-1595298d-1be9-410b-bbe9-96f31c740cb9.png)

- Frequently raised in the earnings call:
  - general economy: basis points (BPS), currency, and inflation
  - Catastrophe: storms, floods, wire fires, and earthquakes
<img width="564" alt="Screenshot 2022-09-07 at 4 53 11 PM" src="https://user-images.githubusercontent.com/61338647/188923557-ff742280-40fe-4bee-8cc9-048159550e76.png">

- Covid, pandemic, and lockdown frequently appear in different topics
- Cross-topic and with a deep influence
<img width="795" alt="image" src="https://user-images.githubusercontent.com/61338647/188924239-1d9ac9b4-e694-477f-be45-308f9d663339.png">

## Result of latent Dirichlet allocation topic modeling (LDA)
- Removed special symbols and numbers.
- Converted all words to lowercase
- Applied tagger to extract only noun words in the lemmatization 
- Expanded the stopwords 
- Paragraph length and remove paragraphs with sentence lengths less than four
- Removed high-frequency tokens
- Processed the documents to join the tokens associated with bi-grams or tri-grams
- Wrapped the post-processed documents in corpus and input them into the LDA model 
<img width="836" alt="image" src="https://user-images.githubusercontent.com/61338647/188924815-4fd35d79-cafc-4661-8625-a85e64c957b4.png">
- words like “capital”, “growth”, and “company” are redundant  
- remove high-frequency words for:
  - Management Discussion of 50 words
  - Questions and Answers of 150 words
<img width="651" alt="image" src="https://user-images.githubusercontent.com/61338647/188924965-6825ef3a-fffd-47c5-97a2-32e7bdc710ea.png">



