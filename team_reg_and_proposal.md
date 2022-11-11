Proposal: Evaluating Nutritional Content of Top National Food Chains in
New York City (2008-2020)
================
2022-11-10

## Group Members

-   Raenita Spriggs (rs4390)
-   Kevin Patterson (kpp2126)
-   Lindsey Covell (ltc2121)
-   Gabriela Jackson (glij2117)
-   Alana Ferris (af3341)

## Motivation for the Project

The growing number of fast-food chains in the United States has pushed
the US into an era of food “convenience.” Since the industry’s inception
in 1927, there are approximately 150 thousand convenience stores across
the US as of
2020.<sup>[1](https://www.emerald.com/insight/content/doi/10.1108/EUM0000000002953/full/html),[2](https://www.statista.com/topics/3869/convenience-stores-in-the-us/),[3](https://www.convenience.org/Research/FactSheets/IndustryStoreCount)</sup>
Their presence is ubiquitous; however, little is known about the general
distribution of fast-food chains in the US. Spatial access to
convenience stores from schools in low and high-income neighborhoods,
and dietary quality have been explored.
<sup>[4](https://escholarship.org/uc/item/93f0g6z8),[5](https://link.springer.com/article/10.1007/s12061-013-9095-6),[6](https://www.frontiersin.org/articles/10.3389/fpubh.2022.857754/full)</sup>
In cities like New York, there seems to be a new chain on every corner
of the city. They provide quick and cheap food options, alongside fast
food chains, which could be the only option for many communities.

Convenience stores and others alike are known to sell food products high
in fats, sugars, and
salts.<sup>[7](https://pubmed.ncbi.nlm.nih.gov/22898159/)</sup> The
presence of convenience stores is associated with higher BMI, higher
obesity, and increased
hypertension.<sup>[8](https://pubmed.ncbi.nlm.nih.gov/16530621/),[9](https://pubmed.ncbi.nlm.nih.gov/17884578/)</sup>
Residents of color living in rural, low-income neighborhoods have
inadequate access to supermarkets, chain grocery stores, and diversity
in food
products.<sup>[10](https://www.ajpmonline.org/article/S0749-3797(08)00838-6/fulltext)</sup>
We are motivated by these findings to investigate trends in NYC.

Our project seeks to investigate at the zip-code level in New York, NY
the general spatial distribution of convenience stores in relation to
demographic composition trends of nutritional content of food served
across years (2008-2020).

## Intended Final Products

-   A report containing the introduction, methods, results, conclusions,
    and future directions
-   A dashboard showcasing maps for NYC at the zip code level

## Anticipated data sources

-   [NYC DOHMH MenuStat nutritional
    database](https://www.menustat.org/data.html)
-   [NYC DOHMH Restaurant Inspections
    database](https://data.cityofnewyork.us/Health/Restaurants-rolled-up-/59dk-tdhz/data)
-   [NY U.S. census, subsetted for
    NYC](https://www.nyc.gov/site/doh/data/data-sets/new-york-city-health-and-nutrition-examination-survey-documentation.page)

## Planned analyses

-   OLS regressions at the zip code level estimating

## Visualizations

-   Box plot of nutritional content by food category and restaurant type
    across combined years (2008-2020)
-   Spaghetti plot of nutritional content by restaurant and coded by
    restaurant type
-   Bar plots of top 15 NYC restaurant chains
-   Maps stratified by restaurant type illustrating restaurants with the
    most/least nutrient-dense menu items according to a national
    standard diet for the average adult (CDC MyPlate).

## Coding Challenges

-   Significant missingness for 10 nutritional variables (`Total_fat`,
    `Saturated_fat`, `Trans_fat`, `Cholesterol`, `Sodium`, `Potassium`,
    `Carbohydrates`, `Protein`, `Sugar`, `Dietary_fiber`); could be
    addressed using conditional mean imputation depending on differences
    in missingness based on food category.
-   An idea of the number of NA’s in 2018 alone:

| serving_size | serving_size_text | serving_size_unit | serving_size_household | calories | total_fat | saturated_fat | trans_fat | cholesterol | sodium | potassium | carbohydrates | protein | sugar | dietary_fiber | calories_100g | total_fat_100g | saturated_fat_100g | trans_fat_100g | cholesterol_100g | sodium_100g | potassium_100g | carbohydrates_100g | protein_100g | sugar_100g | dietary_fiber_100g | calories_text | total_fat_text | saturated_fat_text | trans_fat_text | cholesterol_text | sodium_text | potassium_text | carbohydrates_text | protein_text | sugar_text | dietary_fiber_text |
|-------------:|------------------:|------------------:|-----------------------:|---------:|----------:|--------------:|----------:|------------:|-------:|----------:|--------------:|--------:|------:|--------------:|--------------:|---------------:|-------------------:|---------------:|-----------------:|------------:|---------------:|-------------------:|-------------:|-----------:|-------------------:|--------------:|---------------:|-------------------:|---------------:|-----------------:|------------:|---------------:|-------------------:|-------------:|-----------:|-------------------:|
|        18237 |             30120 |             18225 |                  22061 |     3496 |      3695 |          3708 |      5147 |        4089 |   3572 |     29682 |          3867 |    3899 |  4080 |          4195 |         18545 |          18675 |              18677 |          19534 |            18739 |       18552 |          29855 |              18721 |        18745 |      18667 |              18786 |         29950 |          30120 |              30120 |          30120 |            29967 |       30120 |          30120 |              29833 |        29933 |      29883 |              29786 |

-   MenuStat dataframe doesn’t have location ID; potentially join
    dataframe on
-   Create factor vector that indicates restaurant type: fast food,
    convenience store, sit-down restaurant

## Timeline

| Date        | Task                                         | Due                |
|:------------|:---------------------------------------------|:-------------------|
| Nov 7-10    | Brainstorm                                   | \-                 |
| Nov 10      | Finish draft proposal                        | \-                 |
| Nov 11      | Submit proposal                              | Nov 12 by 1:00 pm  |
| Nov 14      | Designate tasks                              | End of day         |
| Nov 15 - 17 | Cleaning Data                                | Nov 15-17          |
| Nov 15/16   | Project Review Meeting                       | Nov 15 or 16       |
| Nov 18      | Start Analysis                               | \-                 |
| Dec 5       | Finalize code                                | \-                 |
| Dec 6       | Begin and upload website                     | End of day         |
| Dec 10      | Report, webpage, screencast, peer assessment | Dec 10 by 11:59 pm |
| Dec 16      | In class discussion                          | Dec 15             |
