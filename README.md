# recipes-datasets
### Links to datasets on recipes and foods for recipe_recsys project

Nov 3: decide to go with Recipe Box; possibly also trying OpenRecipes download if needed. Added FlavorNetwork paper

Aug 26: Best data sets and related projects found so far are in **bold**

* Kaggle - Using ingredients to categorize cuisine, in JSON (from **[What's Cooking](https://www.kaggle.com/c/whats-cooking/data) competition data**)

https://www.kaggle.com/kaggle/recipe-ingredients-dataset/home * -- previously downloaded data (15.3MB, in JSON), but this link no longer works! Use 2MB what's cooking data instead?

Good dataset to start with (from Kaggle playground competition) 

(June 27: **problem** - no recipe name! just id number and list of ingredients - still continue working with it because it is the smallest and cleanest recipe dataset we found so far)

Related projects:

   * Forked on Kaggle (learn algorithms):  Cuisine classifier *
https://www.kaggle.com/xinrucheng/cuisine-classification-with-accuracy-78-88/edit (Original: https://www.kaggle.com/rahulsridhar2811/cuisine-classification-with-accuracy-78-88)

   * Top 10 most used ingredients (improve with word-stemming)
https://www.kaggle.com/manuelatadvice/noname - simple starter code, using original What's Cooking dataset (id, ingredients and *cuisine type, i.e. Indian*)
   * **Cultural Diffusion by recipe**s https://www.kaggle.com/alonalevy/cultural-diffusion-by-recipes (original What's Cooking dataset)

   * Cluster food by cuisine - using Kmeans, read less readable? also has bugs
https://www.kaggle.com/vincentclaes/clustering-food-by-cuisine

   * Word2Vec with ingredients https://www.kaggle.com/ccorbi/word2vec-with-ingredients (comments in data cleaning and exploration were helpful, but unclear how they got from finding similar vectorized *ingredients* to clustering *cuisines*)
   


* Reddit - a collection of food dataset links (also look into flavor profile repo)

https://www.reddit.com/r/datasets/comments/8nc1d3/is_there_a_dataset_for_a_list_of_all_foods/

  * Flavor network project https://github.com/lingcheng99/Flavor-Network * -- [original paper](http://www.yongyeol.com/papers/ahn-flavornet-2011.pdf) in Network Science on flavour networks is quite interesting! Also repo author mentioned using their data - worth looking into
  
  

* **recipe box: Scrape of ~125,000 recipes (with cooking instructions) from various food websites, 70,000 have associated images** (50.9 MB download, 204.6 MB unzipped, JSON)
https://eightportions.com/datasets/Recipes/#fn:1 [repo here](https://github.com/rtlee9/recipe-box)



* Scrape of recipes from various websites (Epicurious, BBC, Allrecipes and Cookstr) (- June 27: having trouble opening downloaded zipped files?)

https://www.reddit.com/r/datasets/comments/94awca/thousands_of_recipes_from_epicurious_bbc/

* OpenRecipes repo - dump of 173278 recipes in JSON - a database of recipe bookmarks *without* food preparation instructions 
(archived, Punchfork shutdown, "download DB dump" link doesn't work)
https://github.com/fictivekin/openrecipes     
  - **a link in issues points to latest working file form 2017, try to download using wget?** https://github.com/fictivekin/openrecipes/issues/218#issuecomment-304931161

   * Seems to be the same crawl here, **140,000 English Recipes** in computer-readable form with photos (same 4 sites, in HTML and JSON): https://archive.org/details/recipes-en-201706 *  

   * related project looking at 3 decades of Epicurious food data (to look at food trends?):
  https://www.ceros.com/originals/epicurious-recipes-ingredients-part-2/



### Related:

10000 foods (grocery items with brands) with ingredients and weight (from datafiniti, uploaded to data.world) 5.1MB
https://data.world/datafiniti/food-ingredient-lists


OpenFoodFacts website - this looks promising?* 

https://www.reddit.com/r/datasets/comments/3y560h/open_food_facts_database_information_and_data_on/

It's also for commercial food products, but can search by country (see https://world.openfoodfacts.org/discover)

Small Kaggle dataset scraped from online stores, classifying food products for restricted diets
https://www.kaggle.com/theriley106/foodclassification/



Technical article from NYTimes: "Extracting Structured Data From Recipes Using Conditional Random Fields" *

   * Comments are very interesting also (found their (archived) GitHub code there)
https://open.blogs.nytimes.com/2015/04/09/extracting-structured-data-from-recipes-using-conditional-random-fields/

   * https://github.com/nytimes/ingredient-phrase-tagger
NYTimes Cooking has a database of 17000+ recipes at the time of writing (April 2015) -- no ingredient name or list, just index and instructions

   * Also someone commented they made a related API:

  > "The spoonacular Nutrition, Recipe, and Food API allows you to access over 365,000 recipes and 86,000 food products. Our food ontology and semantic recipe search engine makes it possible to search for recipes using natural language queries"
   * https://rapidapi.com/spoonacular/api/recipe-food-nutrition?utm_source=mashape&utm_medium=301#parse-ingredients



Kaggle dataset: 568454 fine food reviews from Amazon, from 1999 to 2012 (SQLite)
https://www.kaggle.com/snap/amazon-fine-food-reviews

(quite a few sentiment analysis projects, but someone did build a prediction system out of it - see top kernel) also fine foods here seem like fancy snacks and condiments with brands, not foods for recipes 


Reddit thread requesting labelled images of food:
("the keyword to search is grocery")
Link to multiple datasets or image recognition on grocery items (also mainly branded grocery items)
https://www.reddit.com/r/datasets/comments/99lwyo/searching_labeled_food_dataset/

US Food & Drug Admin (FDA), someone suggested on Reddit to go there to look for food/nutrition data?
https://open.fda.gov/

* NYT ingredient tagger - modified for Python in manugarri's blog

https://github.com/NYTimes/ingredient-phrase-tagger

http://blog.manugarri.com/nyt_tagger/

recent fork with bug fixes:
https://github.com/mtlynch/ingredient-phrase-tagger



