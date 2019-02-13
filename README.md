# Data-Wrangling-Data-Cleaning-using-Python-Pandas
Cleaning data using python's panda

## This is the Second Series of Data Science Project Series
To get started, download or clone the [first repository (Data Scraping IMDb)](https://github.com/Reljod/Python-Data-Scraping-IMDb-Movie-site-using-BeautifulSoup-Series-1-). It will serve as the source of our dataset.<br>
![clone](https://github.com/Reljod/Data-Wrangling-Data-Cleaning-using-Python-Pandas/blob/master/images/clone.png)
```
git clone https://github.com/Reljod/Python-Data-Scraping-IMDb-Movie-site-using-BeautifulSoup-Series-1-.git
```
### Rename the folder file name to a shorter one
![imagefolder](https://github.com/Reljod/Data-Wrangling-Data-Cleaning-using-Python-Pandas/blob/master/images/folder.png)<br>
![imagenewfolder](https://github.com/Reljod/Data-Wrangling-Data-Cleaning-using-Python-Pandas/blob/master/images/newfolder.png)

## Importing the Data Scraping python file in Jupyter Notebook
#### Installing Jupyter Notebook
If you already installed  the Jupyter Notebook, skip this part.<br>
In cmd or terminal:
```
#On Windows
pip install jupyter
#On Linux
sudo apt-get jupyter
```
#### Change file directory
Go to the folder and copy the file location of imdbData.py file
Open Command Prompt (Windows) or Terminal (Linux or Mac) and change the directory to the file folder or the copied folder
```
cd ..\..\imdbData (depends on where you put the folder)
```
From the directory, open the <b>Jupyter Notebook.</b>
```
#Just type the following:
>>jupyter notebook
```
It should display this:<br>
![jupyter_image](https://github.com/Reljod/Data-Wrangling-Data-Cleaning-using-Python-Pandas/blob/master/images/jupyternoteimage.png)
Select New then click Python3

## Code
Import required packages
```
import pandas as pd
import numpy as np
```
Import the python file that we did in Series 1
```
import imdbData
```
## Extract data from imdbData python file
Open the file and look at its <b>functions</b> and its <b>classes</b>
We need to first get the url before running the main class because the argument of the imdb class needs to have the url
```
url = imdbData.getURL()
```
Now, feed the url to the imdb class
```
data1 = imdbData.IMDB(url)
```
The data1 will be the object that contains the data of the website that we've extracted
## Extracting the data
Get Article Title
```
data1.articleTitle()
```
Get the Movie Data
```
moviedata = data1.movieData()
```

