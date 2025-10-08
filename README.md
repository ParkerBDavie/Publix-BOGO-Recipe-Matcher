# Publix-BOGO-Recipe-Matcher
The goal of this notebook is to explore Publix BOGO items choices and improve weekly grocery shopping, by matching Publix BOGO deals with recipes that use the discounted ingredients.

##Overview
Publix offers "Buy One Get One" deals for ingredients that update weekly and vary by region. The Eight Portions recipe dataset (https://eightportions.com/datasets/Recipes/) is used and compared to the BOGO ingredients via NLP, to find the recipes with the most ingredients on sale for that week.

##In this project
1. BOGO items are scraped directly from the Publix website via Selenium and BeautifulSoup.
2. Recipes are loaded from zip file.
3. Data is cleaned and prepared for NLP.
4. Recipe embeddings are precomputed and stored, in order to lower subsequent run times.
5. Natural language processing (sentence_transformers) is used to match BOGO items to recipe ingredients.
6. Recipes are ranked by number of matches.
7. Data is explored and optimal meals are found.
