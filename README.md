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
<img width="643" alt="image" src="https://user-images.githubusercontent.com/61338647/188923463-479b9263-45d4-42b9-b271-ccef1b921f9e.png">

- Frequently raised in the earnings call:
  - general economy: basis points (BPS), currency, and inflation
  - Catastrophe: storms, floods, wire fires, and earthquakes
<img width="564" alt="Screenshot 2022-09-07 at 4 53 11 PM" src="https://user-images.githubusercontent.com/61338647/188923557-ff742280-40fe-4bee-8cc9-048159550e76.png">

