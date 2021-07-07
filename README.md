# Jerry Thomas' Own Wiki
All cocktail databases are either commercial, or not open data. This is stupid. So, I'm going to write some software to produce a free, open source, and open data cocktail wiki/database.

## Principles
1. Data should be semantic and structured. Ingredients lists should not be just text (which makes scraping reddit hard).
2. Measurements should be consistent and laid out at the outset: Conversions should be easy, but the measurements should be metric/imperial agnostic.
  - parts instead of ounces or ml
  - dashes
  - drops
  - barspoons
3. All data needs to be published daily for an easy download in a variety of formats (csv, json, yml, etc.)
4. An easy to query API using REST
5. Voting. Once a recipe is submitted it is eternal. No edits. Voting is what makes things rise to the top. Perhaps you can edit it within 30 minutes? There has to be some restriction on editing. "Definitive Versions" shall come from upvotes.
6. We really need the ability to get more than just cocktail recipes, i.e. also structured ways to represent syrups and infusions and bitters, etc.
7. Tagging should be encouraged. But tags themselves should be consistent. The system should auto tag anything it can (e.g., citrus).
8. Users should be able to specify shaken or stirred but shaken or stirred should still be autosuggested based on ingredients (e.g., the presence of citrus or cream).
9. Directions should not be the standard drink directions. They should be special instructions. This is for specs, not recipes.


## Steps
1. Get initial data: this may require some legal research, but it looks like Wikipedia's Bartender Wikibook and Webtender are good first starts. Another possibility is scraping r/cocktails and using NLP to convert the data. Finally, I have to look at the legal restrictions, but I may get data from cocktaildb and/or kindred cocktails. Finally, I'm going to look into licensing with sites like Punch and Liquor.com.
2. Build an API
3. Build an app with barcode scanning capabilities. This could be tough and/or expensive.
4. Tell people about it.
