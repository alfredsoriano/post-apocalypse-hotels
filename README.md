# Post Apocalypse Hotels
## Inspiration
*Did you experience the 5th wave and need shelter, supplies, and entertainment?*  
*Are you tired of scavenging for food, water, and beds?*  
*Want to be part of a community again after most of humanity have been taken over by aliens?*  

The answer to all of these can be found at **hotels**!

While it depends on the hotel, as some can be poor, one-star motels while others can be grand, five-star resorts,
they all at the very least offer shelter and a bed. Many hotels, especially in urban areas, offer food from their lounges or restaurants
inside or nearby the hotel. Some hotels can even have pools, TV, arcades, and other entertainment services. Because hotels are designed to be an
"all-in-one" package-- in a fresh post-apocalyptic scenario, I argue to capitalize on the many amenities hotels offer.  

This project looks at cleaning up a large dataset, applying post-processing tools to help visualze geospatial data, and using clustering techniques
to find key areas with an abundance of hotels.

This repository is an assignment from UAA's CSCE A462 Data Mining class,
taught by Dr. Pradeeban Kathiravelu.

## Software
I use **Google Colab** (Jupyter) notebooks, which by default already has many python libraries installed. This is the recommended and intended way to run, view, and edit the code within this repository. Google Colab notebooks can be opened
using Google Colab itself (recommended), or using VSCode. These are the following libraries used:
```
pandas    #used for dataframes and data manipulation
scikit-learn    #used for dbscan clustering algorithm
folium    #used for visualization on maps
```

For the majority of pre-processing, I use **KNIME** as my preferred data mining software.

## Dataset
The original dataset is from Kaggle, from user @raj713335 with the dataset name "Hotels Dataset".  
The link can be found here: 
https://www.kaggle.com/datasets/raj713335/tbo-hotels-dataset  

Note that the original dataset covers multiple countries, so in order to not break Google Colab, I limit the scope
of this project to the United States (including Alaska and Hawaii). I also aim to look at the average hotel ratings
for a given hotel. Therefore, from the original dataset, I remove most attributes such as
"PhoneNumber", "PinCode", "HotelWebsiteUrl", and other irrelevant attributes.  

Below is a random sample of what the cleaned dataset looks like.
|  | Map | stateName | HotelRating |  Latitude |  Longitude |
|---|---|---|---|---|---|
|16125| 32.33016, -106.78285 | New Mexico | 2.0 | 32.330160 | -106.782850 |
|21015| 33.57551, -111.927296  | Arizona | 3.0 | 33.575510 |-111.927296 |
|51809| 40.523094, -105.05278  | Colorado | 2.0 | 40.523094 | -105.052780 |
|61550| 42.6154, -88.58454 | Wisconsin | 3.0 | 42.615400 | -88.584540 |
|56022| 41.32587, -105.60971  | Wyoming | 2.0 | 41.325870 | -105.609710 |
|...|...|...|...|...|...|

## Installation
In a terminal, enter the following command to clone this repository.
```
git clone https://github.com/alfredsoriano/post-apocalypse-hotels.git
```
This repository contains the **.ipynb** (Interactive PYthon NoteBook) file, which can be opened in either
[Google Colab](https://colab.research.google.com/) or VSCode. Once installed, make sure to run the first code block
to import all the needed libraries into the notebook.

If running the code on Google Colab, you can press `ctrl + F9` to run all code blocks in sequence.

## Visualizations
