# DATA512 - A2: Bias in data

# About the Project
In this assignment, the author explored the potential 'bias' that exist in English politicians articles. Specifically, the author analyzed the differences on the coverage of politicians on Wikipedia and the article quality about politicians between various countries. The article qualities are collected by using a machine learning API called [ORES](https://www.mediawiki.org/wiki/ORES) provided by Wikipedia.

# Getting Started
You will need Python 3.X and Jupyter notebook installed to reproduce this project by running _hcds-a2-biasn.ipynb_. 
To install Python 3, see [download](https://www.python.org/downloads/) and [beginner's guide](https://www.python.org/about/gettingstarted/)
To install Jupyter Notebook, follow [installation](http://jupyter.readthedocs.io/en/latest/install.html)

Addtionally, you will need following packages:
* [Pandas](http://pandas.pydata.org)

# Datasets used in this project
## Wikipedia article data

The dataset can be found from [here](https://figshare.com/articles/Untitled_Item/5513449)
__Note__: Please read through the documentation for this repository, then download and unzip it. You will need _page_data.csv_ in the 'data' directory. 
Otherwise, there is a copy of this dataset in this github repo which can be found from [here]()

_page_data.csv_ contains following columns:
1. 'country', country that relates to the article
2. 'page', title of the article
3. 'rev_id', Revision Id, the id to identify the article

## Population Mid 2015 data

The dataset can be found from [Population Research Bureau website](http://www.prb.org/DataFinder/Topic/Rankings.aspx?ind=14)
__Note__: Please look for the 'Microsoft Excel' incon in the upper right and download this data as a CSV file. 

_Population Mid-2015.csv_ contains following columns:
1. 'Location', name of country
2. 'Location Type', type of location, which are all listed as country
3. 'TimeFrame', the time when the data were collected
4. 'Data Type', data type of population, which are all listed as number
5. 'Data', population 
6. 'Footnotes', applicable footnotes, all blank in this dataset

# Using Wikimedia ORES API
In this project, we will use a WikiMedia API called ORES ("Objective Revision Evaluation Service") (See [dcoumentation](https://ores.wikimedia.org/v3/#!/scoring/get_v3_scores_context_revid_model)). ORES estimates the quality of an article (at a particular point in time), and assigns a series of probabilities that the article is in one of 6 quality categories. The options are, from best to worst:

1. FA - Featured article
2. GA - Good article
3. B - B-class article
4. C - C-class article
5. Start - Start-class article
6. Stub - Stub-class article

# License 
* The Wikipedia article data, along with the code used to generate that data, are released under the CC-BY-SA 4.0 license.

* See [About PRB](http://www.prb.org/About.aspx) for the license and copyright information for the population data from Population Reference Bureau 

* By using Wikimedia ORES API, you agree to Wikimedia's [Terms of Use](https://wikimediafoundation.org/wiki/Terms_of_Use/en) and [Privacy Policy](https://wikimediafoundation.org/wiki/Privacy_policy).


This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/HWNi/data-512-a1/blob/master/LICENSE) file for details
