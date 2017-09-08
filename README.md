## ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png)  General Assembly Data Science
### Data Science course DS-SEA-06 Repository
<br><b>Dates: </b>March 20 - May 24
<br><b>Class times:</b> Mon and Wed 6:30pm - 9:30pm</b>
<br><b>Location:</b> Seattle, WA

<b/>Instructor:</b> <a href="https://www.linkedin.com/profile/view?id=ADEAAAEai9UBI1CGmAPFMYpURJeL9zvxWX6xBqI">Jim Byers</a>
<br>
<br>
<!-- **Note:** Prior to the first day of class complete the 10-15 hours of pre-work in order to be properly prepared for class [(prework)](https://gist.github.com/kevinmcalear/9e5625d5eac58fe35de8#account) -->
### Calendar
Monday | Wednesday
--- | ---
**Research Design and Exploratory data analysis**|
3/20: [L01 Introduction to Data Science](#class-1) | 3/22: [L02 Research design and Pandas](#research-design)
3/27: [L03 Statistics fundamentals](#stat_fund) | 3/29: [L04 Command Line and Version Control](#command-line)
4/3: [L05 Fetching Data](#fetching-data), **Project Discussion Deadline** |  
 | 
**Foundations of data modeling**| 
   | | 4/5: [L06 Intro to Classification - K nearest neighbor](#knn), **Project Question and Dataset Due**
4/10: [L07 Intro to Regression](#intro-to-regression) | 4/13: [L08 Evaluating Model Fit](#evaluating-fit)
4/17: [L09 Classifying with Logistic Regression](#logistic-regression) | 4/19: [L10 Advanced model evaluation](#advanced-model)
4/24: [L11 Standardization and Clustering](#clustering) | 4/26: L12 **First Project Presentations** + bonus topics | 
 | 
**Data science in the real world**|
5/1: [L13 Natural Language Processing](#nlp1) | 5/3: [L14 Dimensionality reduction](#reduction), **Draft Paper Due**
5/8 [L15 Decision Trees](#decision) | 5/10: [L16 Ensembling, Bagging and Random Forests](#ensemble)
5/15: [L17 Modeling with Time Series Data I](#time1), **Peer Review Due**| 5/17 [L18 Modeling with Time Series Data II](#time2)
5/22 [L19 Where to go next + bonus topics](#19_topics) | 5/24: **Final Project Presentations** | 
 | 
 | 
 | 
**Bonus Content** | 
Bonus content: [SVC - Support Vector Classifier](#svc) | 
Bonus content: [Naive Bayes Classifier](#bayes)| 
Bonus content: [Intro to Neural Networks](#nn) | 


## Submission Forms

#### [Exit ticket form](https://docs.google.com/a/generalassemb.ly/forms/d/e/1FAIpQLScYwgieGvmvLDEgqtFX_KKtxFWDqbYYkUBroBzZuqbh2RO_cw/viewform)
<!--
(https://docs.google.com/a/generalassemb.ly/forms/d/10L0tgB2X70bIHAzb1d0_4guWmCEqxavhQAHM1t1I4-Y/viewform)
-->
####   [Homework and project submissions form](https://docs.google.com/forms/d/e/1FAIpQLScKCXuRO0q8WQmsO-JYvFiNW6UpdqMsVlzAKXFIQQ9zxbNfXg/viewform)
<!--
(https://docs.google.com/forms/d/1S82LIibhiG2olZQb2C7iboqN5rb8wB6mQLFBg992eh4/viewform?usp=send_form)
-->
* [Homework Evaluation Criteria](https://docs.google.com/spreadsheets/d/19XaVllCETEWyROSMHIShVWgUqK-kbZkvSeCzjK7yezI/edit?usp=sharing)
 &nbsp;

-----

## Other resources

#### [Office hours](other/office_hours.md)

#### [Machine learning estimator selection - a diagram](http://3.bp.blogspot.com/-dofu6J0sZ8o/UrctKb69QdI/AAAAAAAADfg/79ewPecn5XU/s1600/scikit-learn-flow-chart.jpg)

<!-- 
#### [Machine learning model comparison](/other/model_comparison.md) 
 -->
 &nbsp;

-----

<a name="class-1"></a>
### Class 1: Lets get rolling! - Intro to Data Science

**Student Prework**
Before this lesson you should already be able to:
* Define basic data types used in object-oriented programming
* Recall the Python syntax for lists, dictionaries, and functions
* Create files and navigate directories using the command line interface (for your specific environment)

**After this lesson, you will be able to:**
* Describe the roles and components of a successful learning environment
* Define data science and a data science workflow
* Apply the data science workflow to meet your classmates

**Topics/Highlights**
* Welcome from General Assembly!
* Course overview ([slides](slides/01_course_overview.pdf))
* What is data science ([slides](slides/01_data_science_intro.pdf))
* Data Science workflow ([slides](slides/01_data_science_intro.pdf))
	* [Exercise (Apply the workflow)](other/workflow_exercise.md)
* Hands-on with the Data Science Dev Environment (Anaconda, Spyder IDE, iPython notebooks)
* Discuss the course project: [requirements](project/README.md) and [example projects](/project/project_examples/README.md)
	* Types of data ([slides](slides/01_types_of_data.pdf)) and [public data sources](project/public_data.md)
	* [GA's student gallery of projects](https://gallery.generalassemb.ly)

<!--		* Our very own Kevin McAlear's [Hater News DAT project](http://haternews.co/?network=twitter) on the GA gallery
-->
**Homework:**
* Due Mar 22
	* Read through the information about the course project information to familiarize yourself with the [requirements](project/README.md) and [example projects](/project/project_examples/README.md).  Start thinking about what question you would like to answer in your project.
		* Types of data ([slides](slides/01_types_of_data.pdf)) and [public data sources](project/public_data.md)
* Due Mar 27
	* Review each concept and each line of code in these files of python code: [00_python_beginner_workshop.py](code/00_python_beginner_workshop.py) and [00_python_intermediate_workshop.py](code/00_python_intermediate_workshop.py). Complete the coding exercises in the files: If you don't feel comfortable with any of the content (excluding the "requests" and "APIs" sections), you should spend some time before Mar 29 practicing Python.  Use your resources such as documentation, searches, the class Slack to get help if you get stuck. ##Dont
	* To turn in homework,  attach files to a personal message in Slack to Jim Byers and Brandon 
	* Here are some additional resources:
	    * [Introduction to Python](http://introtopython.org/) does a great job explaining Python essentials and includes tons of example code.
	    * If you like learning from a book, [Python for Informatics](http://www.pythonlearn.com/html-270/) has useful chapters on strings, lists, and dictionaries.
	    * If you prefer interactive exercises, try these lessons from [Codecademy](http://www.codecademy.com/en/tracks/python): "Python Lists and Dictionaries" and "A Day at the Supermarket".
	    * If you have more time, try missions 2 and 3 from [DataQuest's Learning Python](https://www.dataquest.io/course/learning-python) course.
	    * If you've already mastered these topics and want more of a challenge, try solving [Python Challenge](http://www.pythonchallenge.com/) number 1 (decoding a message)

**Resources:**
* For a useful look at the different types of data scientists, read [Analyzing the Analyzers](http://cdn.oreillystatic.com/oreilly/radarreport/0636920029014/Analyzing_the_Analyzers.pdf) (32 pages).
* For some thoughts on what it's like to be a data scientist, read these short posts from [Win-Vector](http://www.win-vector.com/blog/2012/09/on-being-a-data-scientist/) and [Datascope Analytics](http://datascopeanalytics.com/what-we-think/2014/07/31/six-qualities-of-a-great-data-scientist).
* Quora has a [data science topic FAQ](https://www.quora.com/Data-Science) with lots of interesting Q&A.

-----

<a name="research-design"></a>
### Class 2: Research Design and Pandas
<!--**Student pre-work**
Before this lesson, you should already be able to:
* Have completed the python pre-work in the class pre-work described [here](https://gist.github.com/kevinmcalear/9e5625d5eac58fe35de8#account) -->

<!-- * Create, open, create and shutdown an IPython Notebook-->

**After this lesson, you will be able to:**
* Define a problem clearly
* Identify data set types
* Apply the data science workflow in the pandas context
* Write an IPython Notebook to import, format and clean data using the Pandas Library

**Topics/Highlights**
* Hands-on with the Data Science Dev Environment (Anaconda, Spyder IDE, iPython notebooks)
* The why's and how's of a good question ([slides](slides/02-experimental-design-and-pandas.pdf))
* The two categories of datasets ([slides](slides/02-experimental-design-and-pandas.pdf))
* Write a research question with raw data (exercise)
* Data Science Workflow
	* Step 1: Identify the problem
	* Steps 2 and 3: Acquire and Understand the data
		* Acquire and Understand data with Pandas 
		* Pandas concepts ([slides](slides/02-experimental-design-and-pandas.pdf))
		* Pandas codealong ([notebook](notebooks/02_numpy_and_pandas.ipynb))
		* Independent Practice ([notebook](notebooks/02_starter_code.ipynb))
 
**Homework:**
* Due Mar 27
	* To turn in homework,  attach files to a personal message in Slack to Jim Byers and Bronson Shonk
	* Review each concept and each line of code in these files of python code: [00_python_beginner_workshop.py](code/00_python_beginner_workshop.py) and [00_python_intermediate_workshop.py](code/00_python_intermediate_workshop.py). Complete the coding exercises in the files: If you don't feel comfortable with any of the content (excluding the "requests" and "APIs" sections), you should spend some time before Mar 27 practicing Python.  Use your resources such as documentation, searches, the class Slack to get help if you get stuck.  Here are some additional resources:
	    * [Introduction to Python](http://introtopython.org/) does a great job explaining Python essentials and includes tons of example code.
	    * If you like learning from a book, [Python for Informatics](http://www.pythonlearn.com/html-270/) has useful chapters on strings, lists, and dictionaries.
	    * If you prefer interactive exercises, try these lessons from [Codecademy](http://www.codecademy.com/en/tracks/python): "Python Lists and Dictionaries" and "A Day at the Supermarket".
	    * If you have more time, try missions 2 and 3 from [DataQuest's Learning Python](https://www.dataquest.io/course/learning-python) course.
	    * If you've already mastered these topics and want more of a challenge, try solving [Python Challenge](http://www.pythonchallenge.com/) number 1 (decoding a message)
	

**Resources:**

Python resources

* [Want to understand Python's comprehensions? Think in Excel or SQL](http://blog.lerner.co.il/want-to-understand-pythons-comprehensions-think-like-an-accountant/) may be helpful if you are still confused by list comprehensions.
* [My code isn't working](http://www.tecoed.co.uk/uploads/1/4/2/4/14249012/624506_orig.png) is a great flowchart explaining how to debug Python errors.
* [PEP 8](https://www.python.org/dev/peps/pep-0008/) is Python's "classic" style guide, and is worth a read if you want to write readable code that is consistent with the rest of the Python community.
* If you want to understand Python at a deeper level, Ned Batchelder's [Loop Like A Native](http://nedbatchelder.com/text/iter.html) and [Python Names and Values](http://nedbatchelder.com/text/names1.html) are excellent presentations.

Pandas resources

Name | Description
--- | ---
[Official Pandas Tutorials](http://pandas.pydata.org/pandas-docs/stable/tutorials.html) | Wes & Company's selection of tutorials and lectures
[Julia Evans Pandas Cookbook](https://github.com/jvns/pandas-cookbook) | Great resource with eamples from weather, bikes and 311 calls
[Learn Pandas Tutorials](https://bitbucket.org/hrojas/learn-pandas) | A great series of Pandas tutorials from Dave Rojas
[Research Computing Python Data PYNBs](https://github.com/ResearchComputing/Meetup-Fall-2013/tree/master/python) | A super awesome set of python notebooks from a meetup-based course exclusively devoted to pandas

-----

<a name="stat_fund"></a>
### Class 3: Statistics fundamentals
**By the end of this lesson you will be able to:**
* Use NumPy and Pandas libraries to analyze datasets using basic summary statistics: mean, median, mode, max, min, quartile, inter-quartile range, variance, standard deviation, and correlation
* Create data visualizations - including: line graphs, box plots, and histograms- to discern characteristics and trends in a dataset
* Identify a normal distribution within a dataset using summary statistics and visualization

**Topics/Highlights**
* More Pandas	
	* Pandas codealong ([notebook](notebooks/02_numpy_and_pandas.ipynb))
	* Independent Practice ([notebook](notebooks/02_starter_code.ipynb))	
* Statistics refresher
	* Basic Statistics with Pandas
		* Statistics Fundamentals [(slides)](slides/03_statistics_fundamentals.pdf)
		* Code-along [(notebook)](notebooks/03_basic_stats.ipynb)
		* Bonus content: Normality Demo [(notebook)](notebooks/03_statistics_demo.ipynb)
	* Correlation
		* What is correlation? [(slides)](https://github.com/JamesByers/GA-SEA-DAT2/blob/master/slides/03_correlation.pdf)
			* Correlation is not causation (fun with a common misconception!)
		* Visualization with Pandas [(notebook)](notebooks/03_correlation_exercise_ice_cream_and_car_data.ipynb)

<!--* [00_python_beginner_workshop.py](code/00_python_beginner_workshop.py)
	* [00_python_intermediate_workshop.py](code/00_python_intermediate_workshop.py) -->
	
**Homework:**
* Due 3/29
	* *Windows users*, install [Git Bash](http://git-scm.com/download/win) prior to starting the command line pre-class exercise*** as you will need the "bash" type command window on your Windows laptop in order to do the exercise and later to use git
		* We recommend Git Bash instead of Git Shell (which uses Powershell).
		* For Mac users, you will probably be using Terminal, or another command line application of your choice.  It already is a bash type command line interpreter.  No need to load anything.  Git is part of the MAC OS so is already installed and ready to use.
	* Complete GA's friendly [command line tutorial](http://generalassembly.github.io/prework/command-line/#/) using Terminal (Linux/Mac) or Git Bash (Windows)
	* Complete the command line pre-class exercise ([code](code/04_command_line_basics.md)).  You do not need to turn in this homework
	* Find one link to a resource about statistics that you find especially useful and send it in a slack message to the class on Slack.  Note this will not be graded against the [homework evaluation criteria](https://docs.google.com/spreadsheets/d/19XaVllCETEWyROSMHIShVWgUqK-kbZkvSeCzjK7yezI/edit?usp=sharing).

**Statistics Resources:**
* [Descriptions of Statistics terms in a straight forward way](http://stattrek.com/statistics/dictionary.aspx?definition=Probability_density_function) including density plot

**Pandas Resources:**
* To learn more Pandas, read this [three-part tutorial](http://www.gregreda.com/2013/10/26/intro-to-pandas-data-structures/), or review these two excellent (but extremely long) notebooks on Pandas: [introduction](https://github.com/fonnesbeck/Bios8366/blob/master/notebooks/Section2_5-Introduction-to-Pandas.ipynb) and [data wrangling](https://github.com/fonnesbeck/Bios8366/blob/master/notebooks/Section2_6-Data-Wrangling-with-Pandas.ipynb).
* If you want to go really deep into Pandas (and NumPy), read the book [Python for Data Analysis](http://shop.oreilly.com/product/0636920023784.do), written by the creator of Pandas.

<!-- * This notebook demonstrates the different types of [joins in Pandas](notebooks/05_pandas_merge.ipynb), for when you need to figure out how to merge two DataFrames. -->
* This is a nice, short tutorial on [pivot tables](https://beta.oreilly.com/learning/pivot-tables) in Pandas.
* For working with geospatial data in Python, [GeoPandas](http://geopandas.org/index.html) looks promising. This [tutorial](http://michelleful.github.io/code-blog/2015/04/24/sgmap/) uses GeoPandas (and scikit-learn) to build a "linguistic street map" of Singapore.

**Visualization Resources:**
* Watch [Look at Your Data](https://www.youtube.com/watch?v=coNDCIMH8bk) (18 minutes) for an excellent example of why visualization is useful for understanding your data.
* For more on Pandas plotting, read this [notebook](https://github.com/fonnesbeck/Bios8366/blob/master/notebooks/Section2_7-Plotting-with-Pandas.ipynb) or the [visualization page](http://pandas.pydata.org/pandas-docs/stable/visualization.html) from the official Pandas documentation.
* To learn how to customize your plots further, browse through this [notebook on matplotlib](https://github.com/fonnesbeck/Bios8366/blob/master/notebooks/Section2_4-Matplotlib.ipynb) or this [similar notebook](https://github.com/jrjohansson/scientific-python-lectures/blob/master/Lecture-4-Matplotlib.ipynb).
* Read [Overview of Python Visualization Tools](http://pbpython.com/visualization-tools-1.html) for a useful comparison of Matplotlib, Pandas, Seaborn, ggplot, Bokeh, Pygal, and Plotly.
* To explore different types of visualizations and when to use them, [Choosing a Good Chart](http://extremepresentation.typepad.com/files/choosing-a-good-chart-09.pdf) and [The Graphic Continuum](http://www.coolinfographics.com/storage/post-images/The-Graphic-Continuum-POSTER.jpg) are nice one-page references, and the interactive [R Graph Catalog](http://shiny.stat.ubc.ca/r-graph-catalog/) has handy filtering capabilities.
* This [PowerPoint presentation](http://www2.research.att.com/~volinsky/DataMining/Columbia2011/Slides/Topic2-EDAViz.ppt) from Columbia's Data Mining class contains lots of good advice for properly using different types of visualizations.
* [Harvard's Data Science course](http://cs109.github.io/2014/) includes an excellent lecture on [Visualization Goals, Data Types, and Statistical Graphs](http://cm.dce.harvard.edu/2015/01/14328/L03/screen_H264LargeTalkingHead-16x9.shtml) (83 minutes), for which the [slides](https://docs.google.com/file/d/0B7IVstmtIvlHLTdTbXdEVENoRzQ/edit) are also available.

-----

<a name="command-line"></a>
### Class 4: Command Line and Version Control

**By the end of this lesson you will be able to:**
* clone a Githib repository to your laptop
* synch your local files with your GitHub repository using git add, commit, push and pull
* use more advanced command line commands such as Grep and |

**Topics/Highlights**
* Review the command line pre-class exercise ([code](code/04_command_line_basics.md))
* Git and GitHub ([slides](slides/04_git_github.pdf))
* Intermediate command line [(commands)](code/04_command_line_with_intermediate_advanced.md)

**Homework:**
* Due 4/5 Complete the [command line homework assignment](homework/04_command_line_chipotle.md) with the Chipotle data.
* **Optional:** Browse through some more [example student projects](/project/project_examples/README.md), which may help to inspire your own project!

**Git and Markdown Resources:**
* [Pro Git](http://git-scm.com/book/en/v2) is an excellent book for learning Git. Read the first two chapters to gain a deeper understanding of version control and basic commands.
* If you want to practice a lot of Git (and learn many more commands), [Git Immersion](http://gitimmersion.com/) looks promising.
* If you want to understand how to contribute on GitHub, you first have to understand [forks and pull requests](http://www.dataschool.io/simple-guide-to-forks-in-github-and-git/).
* [GitRef](http://gitref.org/) is my favorite reference guide for Git commands, and [Git quick reference for beginners](http://www.dataschool.io/git-quick-reference-for-beginners/) is a shorter guide with commands grouped by workflow.
* [Cracking the Code to GitHub's Growth](https://growthhackers.com/growth-studies/github) explains why GitHub is so popular among developers.
* [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) provides a thorough set of Markdown examples with concise explanations. GitHub's [Mastering Markdown](https://guides.github.com/features/mastering-markdown/) is a simpler and more attractive guide, but is less comprehensive.

**Command Line Resources:**
* If you want to go much deeper into the command line, [Data Science at the Command Line](http://shop.oreilly.com/product/0636920032823.do) is a great book. The [companion website](http://datascienceatthecommandline.com/) provides installation instructions for a "data science toolbox" (a virtual machine with many more command line tools), as well as a long reference guide to popular command line tools.
* If you want to do more at the command line with CSV files, try out [csvkit](http://csvkit.readthedocs.org/), which can be installed via `pip`.

-----

<a name="fetching-data"></a>
### Class 5: Fetching Data

**After this lesson you will be able to:**
* Articulate what JSON, APIs and Web scraping are and how they help us fetch data
* Retrieve data from a website using the site’s APIs

**Topics/Highlights:**
* Fetching data through APIs
    * APIs - key concepts [(slides)](slides/05_APIs_and_web_scraping.pdf)
    * Example of API documentation: [The OMDb API - omdbapi.com](http://www.omdbapi.com/)
    * Code along - Access APIs on omdbapi.com [(code)](code/05_api.py)
    * Exercise - Retrieve US Census language stats though APIs [(code)](code/05_api_census.py)
     * [Census.gov language statistics page with API description](http://www.census.gov/data/developers/data-sets/language-stats.html)
* Bonus content: Grabbing data using Web scraping ([code](code/05_web_scraping.py))
    * [APIs - key concepts (slides)](slides/05_APIs_and_web_scraping.pdf)
    * [IMDb: robots.txt](http://www.imdb.com/robots.txt)
    * [Example web page](data/example.html)
    * [IMDb: The Shawshank Redemption](http://www.imdb.com/title/tt0111161/)

**Homework:**
* Due 4/5 
	* Complete the [command line homework assignment](homework/04_command_line_chipotle.md) with the Chipotle data.
	* If you're using Anaconda, install Seaborn by running `conda install seaborn` at the command line. (Note that some students in past courses have had problems with Anaconda after installing Seaborn.) If you're not using Anaconda, [install Seaborn](http://stanford.edu/~mwaskom/software/seaborn/installing.html) using `pip`. 
	* **Optional:** Complete the homework exercise listed in the [web scraping code](code/05_web_scraping.py). It will take the place of any one homework you miss, past or future! This optional homework is due on April 10.

**API Resources:**
* This Python script to [query the U.S. Census API](https://github.com/laurakurup/census-api) was created by a former DAT student. It's a bit more complicated than the example we used in class, it's very well commented, and it may provide a useful framework for writing your own code to query APIs.
* [Mashape](https://www.mashape.com/explore) and [Apigee](https://apigee.com/providers) allow you to explore tons of different APIs. Alternatively, a [Python API wrapper](http://www.pythonforbeginners.com/api/list-of-python-apis) is available for many popular APIs.
* The [Data Science Toolkit](http://www.datasciencetoolkit.org/) is a collection of location-based and text-related APIs.
* [API Integration in Python](https://realpython.com/blog/python/api-integration-in-python/) provides a very readable introduction to REST APIs.
* Microsoft's [Face Detection API](https://www.projectoxford.ai/demo/face#detection), which powers [How-Old.net](http://how-old.net/), is a great example of how a machine learning API can be leveraged to produce a compelling web application.

**Web Scraping Resources:**
* The [Beautiful Soup documentation](http://www.crummy.com/software/BeautifulSoup/bs4/doc/) is incredibly thorough, but is hard to use as a reference guide. However, the section on [specifying a parser](http://www.crummy.com/software/BeautifulSoup/bs4/doc/#specifying-the-parser-to-use) may be helpful if Beautiful Soup appears to be parsing a page incorrectly.
* For more Beautiful Soup examples and tutorials, see [Web Scraping 101 with Python](http://www.gregreda.com/2013/03/03/web-scraping-101-with-python/), a former DAT student's well-commented notebook on [scraping Craigslist](https://github.com/Alexjmsherman/DataScience_GeneralAssembly/blob/master/Final_Project/1.%20Final_Project_Data%20Scraping.ipynb), this [notebook](http://web.stanford.edu/~zlotnick/TextAsData/Web_Scraping_with_Beautiful_Soup.html) from Stanford's Text As Data course, and this [notebook](https://github.com/cs109/2014/blob/master/lectures/2014_09_23-lecture/data_scraping_transcript.ipynb) and associated [video](http://cm.dce.harvard.edu/2015/01/14328/L07/screen_H264LargeTalkingHead-16x9.shtml) from Harvard's Data Science course.
* For a much longer web scraping tutorial covering Beautiful Soup, lxml, XPath, and Selenium, watch [Web Scraping with Python](https://www.youtube.com/watch?v=p1iX0uxM1w8) (3 hours 23 minutes) from PyCon 2014. The [slides](https://docs.google.com/presentation/d/1uHM_esB13VuSf7O1ScGueisnrtu-6usGFD3fs4z5YCE/edit#slide=id.p) and [code](https://github.com/kjam/python-web-scraping-tutorial) are also available.
* For more complex web scraping projects, [Scrapy](http://scrapy.org/) is a popular application framework that works with Python. It has excellent [documentation](http://doc.scrapy.org/en/1.0/index.html), and here's a [tutorial](https://github.com/rdempsey/ddl-data-wrangling) with detailed slides and code.
* [robotstxt.org](http://www.robotstxt.org/robotstxt.html) has a concise explanation of how to write (and read) the `robots.txt` file.
* [import.io](https://import.io/) and [Kimono](https://www.kimonolabs.com/) claim to allow you to scrape websites without writing any code.
* [How a Math Genius Hacked OkCupid to Find True Love](http://www.wired.com/2014/01/how-to-hack-okcupid/all/) and [How Netflix Reverse Engineered Hollywood](http://www.theatlantic.com/technology/archive/2014/01/how-netflix-reverse-engineered-hollywood/282679/?single_page=true) are two fun examples of how web scraping has been used to build interesting datasets.

-----

<a name="knn"></a>
### Class 6: K-Nearest Neighbors

**After this lesson you will be able to:**
* Indentify the steps to build a predictive model in scikit-learn
* Create a k nearest neighbors (knn) predictive model
* Describe the difference between a supervised and unsupervised model

**Topics/Highlights:***
* Chipotle command line homework due [(code)](homework/04_command_line_chipotle.md)
* K-nearest neighbors (KNN) and scikit-learn ([notebook](notebooks/06_knn_sklearn.ipynb))
* Exercise with NBA player data ([notebook](notebooks/06_nba_knn.ipynb), [data](/data/NBA_players_2015.csv), [data dictionary](/slides/06_nba_paper.pdf))
* Bonus content not covered in this lesson: Machine learning types and terms [(slides)](slides/06_machine_learning.pdf) 

**Homework:**
* Due 4/12: Complete this [homework assignment](homework/06_yelp_votes_homework.ipynb) with the [Yelp data](data/yelp.csv)

**KNN Resources:**
* [(notebook)](notebooks/07_human_learning_iris.ipynb) An example of the steps one would go through using "human learning" to come up with a rule to classify new iris observations based on the Iris data set.  Contains a refresher on many Pandas techniques such as groupby and visualization.
* For a recap of the key points about KNN and scikit-learn, watch [Getting started in scikit-learn with the famous iris dataset](https://www.youtube.com/watch?v=hd1W4CyPX58) (15 minutes) and [Training a machine learning model with scikit-learn](https://www.youtube.com/watch?v=RlQuVL6-qe8) (20 minutes).
* KNN supports [distance metrics](http://scikit-learn.org/stable/modules/generated/sklearn.neighbors.DistanceMetric.html) other than Euclidean distance, such as [Mahalanobis distance](http://stats.stackexchange.com/questions/62092/bottom-to-top-explanation-of-the-mahalanobis-distance), which [takes the scale of the data into account](http://blogs.sas.com/content/iml/2012/02/15/what-is-mahalanobis-distance.html).
* [A Detailed Introduction to KNN](https://saravananthirumuruganathan.wordpress.com/2010/05/17/a-detailed-introduction-to-k-nearest-neighbor-knn-algorithm/) is a bit dense, but provides a more thorough introduction to KNN and its applications.
* This lecture on [Image Classification](http://cs231n.github.io/classification/) shows how KNN could be used for detecting similar images, and also touches on topics we will cover in future classes (hyperparameter tuning and cross-validation).
* Some applications for which KNN is well-suited are [object recognition](http://vlm1.uta.edu/~athitsos/nearest_neighbors/), [satellite image enhancement](http://land.umn.edu/documents/FS6.pdf), [document categorization](http://www.ceng.metu.edu.tr/~e120321/paper.pdf), and [gene expression analysis](http://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.208.993).

**Seaborn Resources:**
* The official Seaborn website has a series of [detailed tutorials](http://web.stanford.edu/~mwaskom/software/seaborn/tutorial.html) and an [example gallery](http://web.stanford.edu/~mwaskom/software/seaborn/examples/index.html).
* [Data visualization with Seaborn](https://beta.oreilly.com/learning/data-visualization-with-seaborn) is a quick tour of some of the popular types of Seaborn plots.
* [Visualizing Google Forms Data with Seaborn](http://pbpython.com/pandas-google-forms-part2.html) and [How to Create NBA Shot Charts in Python](http://savvastjortjoglou.com/nba-shot-sharts.html) are both good examples of Seaborn usage on real-world data.

-----

<a name="intro-to-regression"></a>
### Class 7: Intro to regression

**After this lesson you will be able to:**
* Indentify the kinds of problems that Linear Regression can solve
* Create a linear regression predictive model
* Evaluate the error of the model's fit to the training data

**Topics/Highlights:**
* Linear regression ([notebook](notebooks/07_linear_regression.ipynb))
    * [Capital Bikeshare dataset](data/bikeshare.csv) used in a Kaggle competition
    * [Data dictionary](https://www.kaggle.com/c/bike-sharing-demand/data)
* Why we should examine data well before building a model: Anscombes_Quartet [(notebook)](notebooks/06_Anscombes_Quartet.ipynb)

<!--* An additional feature engineering example is available here: [Predicting User Engagement in Corporate Collaboration Network](https://github.com/mikeyea/DAT7_project/blob/master/final%20project/Class_Presention_MYea.ipynb) -->

**Homework:**
* The [homework assignment](homework/06_yelp_votes_homework.ipynb) with the [Yelp data](data/yelp.csv) is due 4/12
* Reading assignment on the [bias-variance tradeoff](homework/08_bias_variance.md)
* Read Kevin Markhams's [introduction to reproducibility](http://www.dataschool.io/reproducibility-is-not-just-for-researchers/), read Jeff Leek's [guide to creating a reproducible analysis](https://github.com/jtleek/datasharing), and watch this related [Colbert Report video](http://thecolbertreport.cc.com/videos/dcyvro/austerity-s-spreadsheet-error) (8 minutes).
* Optional: Quick Pandas exercise ([notebook](notebooks/08_pandas_review.ipynb)).  Complete this exercise to sharpen your understanding of dataframes.
* Work on your project... your first project presentation is in less than three weeks!


**Linear Regression Resources:**
* To go much more in-depth on linear regression, read Chapter 3 of [An Introduction to Statistical Learning](http://www-bcf.usc.edu/~gareth/ISL/). Alternatively, watch the [related videos](http://www.dataschool.io/15-hours-of-expert-machine-learning-videos/) or read Kevin Markhams [quick reference guide](http://www.dataschool.io/applying-and-interpreting-linear-regression/) to the key points in that chapter.
* This [introduction to linear regression](http://people.duke.edu/~rnau/regintro.htm) is more detailed and mathematically thorough, and includes lots of good advice.
* This is a relatively quick post on the [assumptions of linear regression](http://pareonline.net/getvn.asp?n=2&v=8).
* Setosa has an [interactive visualization](http://setosa.io/ev/ordinary-least-squares-regression/) of linear regression.

**Seaborn Resources:**
* The official Seaborn website has a series of [detailed tutorials](http://web.stanford.edu/~mwaskom/software/seaborn/tutorial.html) and an [example gallery](http://web.stanford.edu/~mwaskom/software/seaborn/examples/index.html).
* [Data visualization with Seaborn](https://beta.oreilly.com/learning/data-visualization-with-seaborn) is a quick tour of some of the popular types of Seaborn plots.
* [Visualizing Google Forms Data with Seaborn](http://pbpython.com/pandas-google-forms-part2.html) and [How to Create NBA Shot Charts in Python](http://savvastjortjoglou.com/nba-shot-sharts.html) are both good examples of Seaborn usage on real-world data.
<!--* Types of data ([slides](slides/01_types_of_data.pdf)) and [public data sources](project/public_data.md)
* Discuss the course project: [requirements](project/README.md) and [example projects](/project/project_examples/README.md) -->

-----

<a name="evaluating-fit"></a>
### Class 8: Basic Model Evaluation

**After this lesson you will be able to:**
* Describe what Bias and Variance are
* Explain the Bias/Variance tradeoff
* Assess overall model accuracy with test/train split data

**Topics/Highlights:**
* Discuss the reading assignment on the [bias-variance tradeoff](homework/08_bias_variance.md)
* Exploring the bias-variance tradeoff ([notebook](notebooks/08_bias_variance.ipynb)) 
* Model evaluation using train/test split ([notebook](notebooks/08_model_evaluation.ipynb))
* Exploring the scikit-learn documentation: [module reference](http://scikit-learn.org/stable/modules/classes.html), [user guide](http://scikit-learn.org/stable/user_guide.html), class and function documentation
* Bonus content: Reproducibility
	* Discuss assigned readings: [introduction](http://www.dataschool.io/reproducibility-is-not-just-for-researchers/), [Colbert Report video](http://thecolbertreport.cc.com/videos/dcyvro/austerity-s-spreadsheet-error), [cabs article](http://iquantny.tumblr.com/post/107245431809/how-software-in-half-of-nyc-cabs-generates-5-2), [Tweet](https://twitter.com/jakevdp/status/519563939177197571), [creating a reproducible analysis](https://github.com/jtleek/datasharing)
	* Examples: [Classic rock](https://github.com/fivethirtyeight/data/tree/master/classic-rock), [student project 1](https://github.com/jwknobloch/DAT4_final_project)

<!--
**Homework:**
* Watch [Data science in Python](https://www.youtube.com/watch?v=3ZWuPVWq7p4) (35 minutes) for an introduction to linear regression (and a review of other course content), or at the very least, read through the [associated notebook](https://github.com/justmarkham/scikit-learn-videos/blob/master/06_linear_regression.ipynb).
* **Optional:** For another introduction to linear regression, watch [The Easiest Introduction to Regression Analysis](https://www.youtube.com/watch?v=k_OB1tWX9PM) (14 minutes).
-->
**Model Evaluation Resources:**
* For a recap of some of the key points of model evaluation, watch [Comparing machine learning models in scikit-learn](https://www.youtube.com/watch?v=0pP4EwWJgIU) (27 minutes).
* For another explanation of training error versus testing error, the bias-variance tradeoff, and train/test split (also known as the "validation set approach"), watch Hastie and Tibshirani's video on [estimating prediction error](https://www.youtube.com/watch?v=_2ij6eaaSl0&t=2m34s) (12 minutes, starting at 2:34).
* Caltech's Learning From Data course includes a fantastic video on [visualizing bias and variance](http://work.caltech.edu/library/081.html) (15 minutes).
* [Random Test/Train Split is Not Always Enough](http://www.win-vector.com/blog/2015/01/random-testtrain-split-is-not-always-enough/) explains why random train/test split may not be a suitable model evaluation procedure if your data has a significant time element.

**Reproducibility Resources:**
* [What We've Learned About Sharing Our Data Analysis](https://source.opennews.org/en-US/articles/what-weve-learned-about-sharing-our-data-analysis/) includes tips from BuzzFeed News about how to publish a reproducible analysis.
* [Software development skills for data scientists](http://treycausey.com/software_dev_skills.html) discusses the importance of writing functions and proper code comments (among other skills), which are highly useful for creating a reproducible analysis.
* [Data science done well looks easy - and that is a big problem for data scientists](http://simplystatistics.org/2015/03/17/data-science-done-well-looks-easy-and-that-is-a-big-problem-for-data-scientists/) explains how a reproducible analysis demonstrates all of the work that goes into proper data science.

-----

<a name="logistic-regression"></a>
### Class 9: Logistic Regression

**After this lesson you will be able to:**
* Describe the kind of problem Logistic regression can solve
* Create a logistic regression model
* Describe the elements of a Confusion Matrix

**Topics/Highlights:**
* Logistic regression ([notebook](notebooks/09_logistic_regression.ipynb))
    * [Glass identification dataset](https://archive.ics.uci.edu/ml/datasets/Glass+Identification)
    * [e and natural log - what are they?](notebooks/09_e_log_examples.ipynb)
* Exercise with Titanic data ([notebook](notebooks/09_titanic_logistic_regression_exercise.ipynb), [data](data/titanic.csv), [data dictionary](https://www.kaggle.com/c/titanic/data))
* Confusion matrix ([slides](slides/09_confusion_matrix.pdf), [notebook](notebooks/09_confusion_matrix.ipynb))

**Homework:**
* Work through the code samples in the "Confusion matrix of Titanic predictions" section in [the 09_confusion_matrix.ipynb notebook](notebooks/09_confusion_matrix.ipynb) to see an example of changing a threshhold to get the desired behavior in the confusion matrix.
* If you aren't yet comfortable with all of the confusion matrix terminology, watch Rahul Patwari's videos on [Intuitive sensitivity and specificity](https://www.youtube.com/watch?v=U4_3fditnWg) (9 minutes) and [The tradeoff between sensitivity and specificity](https://www.youtube.com/watch?v=vtYDyGGeQyo) (13 minutes).
* Video/reading assignment on [ROC curves and AUC](homework/10_roc_auc.md)
* Video/reading assignment on [cross-validation](homework/10_cross_validation.md)

**Logistic Regression Resources:**
* To go deeper into logistic regression, read the first three sections of Chapter 4 of [An Introduction to Statistical Learning](http://www-bcf.usc.edu/~gareth/ISL/), or watch the [first three videos](http://www.dataschool.io/15-hours-of-expert-machine-learning-videos/) (30 minutes) from that chapter.
* For a math-ier explanation of logistic regression, watch the first seven videos (71 minutes) from week 3 of Andrew Ng's [machine learning course](https://www.coursera.org/learn/machine-learning/home/info), or read the [related lecture notes](http://www.holehouse.org/mlclass/06_Logistic_Regression.html) compiled by a student.
* For more on interpreting logistic regression coefficients, read this excellent [guide](http://www.ats.ucla.edu/stat/mult_pkg/faq/general/odds_ratio.htm) by UCLA's IDRE and these [lecture notes](http://www.unm.edu/~schrader/biostat/bio2/Spr06/lec11.pdf) from the University of New Mexico.
* The scikit-learn documentation has a nice [explanation](http://scikit-learn.org/stable/modules/calibration.html) of what it means for a predicted probability to be calibrated.
* [Supervised learning superstitions cheat sheet](http://ryancompton.net/assets/ml_cheat_sheet/supervised_learning.html) is a very nice comparison of four classifiers we cover in the course (logistic regression, decision trees, KNN, Naive Bayes) and one classifier we do not cover (Support Vector Machines).

**Confusion Matrix Resources:**
* Kevin Markham's [simple guide to confusion matrix terminology](http://www.dataschool.io/simple-guide-to-confusion-matrix-terminology/) may be useful to you as a reference.
* This blog post about [Amazon Machine Learning](https://aws.amazon.com/blogs/aws/amazon-machine-learning-make-data-driven-decisions-at-scale/) contains a neat [graphic](https://media.amazonwebservices.com/blog/2015/ml_adjust_model_1.png) showing how classification threshold affects different evaluation metrics.
* This notebook (from another DAT course) explains [how to calculate "expected value"](https://github.com/podopie/DAT18NYC/blob/master/classes/13-expected_value_cost_benefit_analysis.ipynb) from a confusion matrix by treating it as a cost-benefit matrix.

-----

<a name="advanced-model"></a>
### Class 10: Advanced Model Evaluation

**After this lesson you will be able to:**
* Prepare your data by overcoming issues such as null values
* Measure accuracy of Logistic Regression with ROC curves and AUC
* Use cross validation to measure model accuracy more effectively than with test/train split

**Topics/Highlights:**
* Data preparation [(notebook)](notebooks/10_advanced_model_evaluation.ipynb)
    * Handling missing values
    * Handling categorical features (review)
* Advanced Model evaluation
	* ROC curves and AUC
	    * Discuss the [video/reading assignment](homework/10_roc_auc.md)
	    * Exercise: drawing an ROC curve ([slides](slides/10_drawing_roc.pdf))
	    * Return to the main notebook
	* Cross-validation
	    * Discuss the [video/reading assignment](homework/10_cross_validation.md) and related [notebook](notebooks/10_cross_validation.ipynb)
	    * Return to the main notebook
* Exercise with bank marketing data ([notebook](notebooks/10_bank_exercise.ipynb), [data](data/bank-additional.csv), [data dictionary](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing))

**Homework:**
* **Finalize your First Project Presentations!**  Your first project presentation is next Thursday Oct 27.
	* [Requirements for the presentations](/project/README.md)

**ROC Resources:**
* Rahul Patwari has a great video on [ROC Curves](https://www.youtube.com/watch?v=21Igj5Pr6u4) (12 minutes).
* [An introduction to ROC analysis](http://people.inf.elte.hu/kiss/13dwhdm/roc.pdf) is a very readable paper on the topic.
* ROC curves can be used across a wide variety of applications, such as [comparing different feature sets](http://research.microsoft.com/pubs/205472/aisec10-leontjeva.pdf) for detecting fraudulent Skype users, and [comparing different classifiers](http://www.cse.ust.hk/nevinZhangGroup/readings/yi/Bradley_PR97.pdf) on a number of popular datasets.

**Cross-Validation Resources:**
* For more on cross-validation, read section 5.1 of [An Introduction to Statistical Learning](http://www-bcf.usc.edu/~gareth/ISL/) (11 pages) or watch the related videos: [K-fold and leave-one-out cross-validation](https://www.youtube.com/watch?v=nZAM5OXrktY) (14 minutes), [cross-validation the right and wrong ways](https://www.youtube.com/watch?v=S06JpVoNaA0) (10 minutes).
* If you want to understand the different variations of cross-validation, this [paper](http://www.jcheminf.com/content/pdf/1758-2946-6-10.pdf) examines and compares them in detail.
* To learn how to use [GridSearchCV and RandomizedSearchCV](http://scikit-learn.org/stable/modules/grid_search.html) for parameter tuning, watch [How to find the best model parameters in scikit-learn](https://www.youtube.com/watch?v=Gol_qOgRqfA) (28 minutes) or read the [associated notebook](https://github.com/justmarkham/scikit-learn-videos/blob/master/08_grid_search.ipynb).

**Other Resources:**
* scikit-learn has extensive documentation on [model evaluation](http://scikit-learn.org/stable/modules/model_evaluation.html).
* [Counterfactual evaluation of machine learning models](https://www.youtube.com/watch?v=QWCSxAKR-h0) (45 minutes) is an excellent talk about the sophisticated way in which Stripe evaluates its fraud detection model. (These are the associated [slides](http://www.slideshare.net/MichaelManapat/counterfactual-evaluation-of-machine-learning-models).)
* [Visualizing Machine Learning Thresholds to Make Better Business Decisions](http://blog.insightdatalabs.com/visualizing-classifier-thresholds/) demonstrates how visualizing precision, recall, and "queue rate" at different thresholds can help you to maximize the business value of your classifier.

-----

<a name="clustering"></a>
### Class 11: Standardization (z-value scaling) and Clustering
**By the end of this lesson you will be able to:**

* Standardize feature values
* Cluster using K-means
* Compare "how good" the clustering models are

**Topics/Highlights**

* Review solutions to exercise with bank marketing data ([notebook](notebooks/solutions/10_bank_exercise_solutions.ipynb), [data](data/bank-additional.csv), [data dictionary](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing))
* Advanced scikit-learn ([notebook](notebooks/11_advanced_sklearn.ipynb),[dataset description](http://archive.ics.uci.edu/ml/datasets/Wine))
    * [StandardScaler](http://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.StandardScaler.html): standardizing features
    * [Pipeline](http://scikit-learn.org/stable/modules/pipeline.html): chaining steps
* Clustering ([slides](slides/11_clustering.pdf), [notebook](notebooks/11_clustering.ipynb),[data)](https://raw.githubusercontent.com/JamesByers/GA-SEA-DAT2/master/data/beer.txt)
    * K-means: [documentation](http://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html), [visualization 1](http://tech.nitoyon.com/en/blog/2013/11/07/k-means/), [visualization 2](http://www.naftaliharris.com/blog/visualizing-k-means-clustering/)
    	* My clustering of colors in an image to posterize.  Used a loop to generate clusters of 1 to 256 clusters. Made an animated gif out of them.  Fun! [(repository](https://github.com/JamesByers/Cluster-analysis-of-image-RGB-colors),[gif)](https://github.com/JamesByers/Cluster-analysis-of-image-RGB-colors/blob/master/image_output_files/Newport_seafood_k_means%2B%2B_cluster_animated.gif)
    * DBSCAN: [documentation](http://scikit-learn.org/stable/modules/generated/sklearn.cluster.DBSCAN.html), [visualization](http://www.naftaliharris.com/blog/visualizing-dbscan-clustering/)

**Homework:**
* Prepare your initial project presentation for Wednesday!!

<!--
* By Monday August 8, run the "DCSCAN Clustering" part of the [11_clustering.ipynb notebook](notebooks/11_clustering.ipynb) to understand how to use the DBSCAN estimator to build a clustering model.  -->

**scikit-learn Resources:**
* This is a longer example of [feature scaling](https://github.com/rasbt/pattern_classification/blob/master/preprocessing/about_standardization_normalization.ipynb) in scikit-learn, with additional discussion of the types of scaling you can use.
* [Practical Data Science in Python](http://radimrehurek.com/data_science_python/) is a long and well-written notebook that uses a few advanced scikit-learn features: pipelining, plotting a learning curve, and pickling a model.
* To learn how to use [GridSearchCV and RandomizedSearchCV](http://scikit-learn.org/stable/modules/grid_search.html) for parameter tuning, watch [How to find the best model parameters in scikit-learn](https://www.youtube.com/watch?v=Gol_qOgRqfA) (28 minutes) or read the [associated notebook](https://github.com/justmarkham/scikit-learn-videos/blob/master/08_grid_search.ipynb).
* Sebastian Raschka has a number of excellent resources for scikit-learn users, including a repository of [tutorials and examples](https://github.com/rasbt/pattern_classification), a library of machine learning [tools and extensions](http://rasbt.github.io/mlxtend/), a new [book](https://github.com/rasbt/python-machine-learning-book), and a semi-active [blog](http://sebastianraschka.com/blog/).
* scikit-learn has an incredibly active [mailing list](https://www.mail-archive.com/scikit-learn-general@lists.sourceforge.net/index.html) that is often much more useful than Stack Overflow for researching functions and asking questions.
* If you forget how to use a particular scikit-learn function that we have used in class, don't forget that this repository is fully searchable!

**Clustering Resources:**
* For a very thorough introduction to clustering, read chapter 8 (69 pages) of [Introduction to Data Mining](http://www-users.cs.umn.edu/~kumar/dmbook/index.php) (available as a free download), or browse through the chapter 8 slides.
* scikit-learn's user guide compares many different [types of clustering](http://scikit-learn.org/stable/modules/clustering.html).
* This [PowerPoint presentation](http://www2.research.att.com/~volinsky/DataMining/Columbia2011/Slides/Topic6-Clustering.ppt) from Columbia's Data Mining class provides a good introduction to clustering, including hierarchical clustering and alternative distance metrics.
* An Introduction to Statistical Learning has useful videos on [K-means clustering](https://www.youtube.com/watch?v=aIybuNt9ps4&list=PL5-da3qGB5IBC-MneTc9oBZz0C6kNJ-f2) (17 minutes) and [hierarchical clustering](https://www.youtube.com/watch?v=Tuuc9Y06tAc&list=PL5-da3qGB5IBC-MneTc9oBZz0C6kNJ-f2) (15 minutes).
* This is an excellent interactive visualization of [hierarchical clustering](https://joyofdata.shinyapps.io/hclust-shiny/).
* This is a nice animated explanation of [mean shift clustering](http://spin.atomicobject.com/2015/05/26/mean-shift-clustering/).
* The [K-modes algorithm](http://www.cs.ust.hk/~qyang/Teaching/537/Papers/huang98extensions.pdf) can be used for clustering datasets of categorical features without converting them to numerical values. Here is a [Python implementation](https://github.com/nicodv/kmodes).
* Here are some fun examples of clustering: [A Statistical Analysis of the Work of Bob Ross](http://fivethirtyeight.com/features/a-statistical-analysis-of-the-work-of-bob-ross/) (with [data and Python code](https://github.com/fivethirtyeight/data/tree/master/bob-ross)), [How a Math Genius Hacked OkCupid to Find True Love](http://www.wired.com/2014/01/how-to-hack-okcupid/all/), and [characteristics of your zip code](http://www.esri.com/landing-pages/tapestry/).

-----

<a name="nlp1"></a>
### Class 13: Natural Language Processing
**By the end of this lesson you will be able to:**

* Apply the NLP techniques of Vectorization and Tokenization to text to create features
* Use stop word removal and other techniques to increase the accuracy of your models using these features
* Create features using Stemming and Lemmatization

**Topics/Highlights**

* Natural language processing ([notebook](notebooks/13_natural_language_processing.ipynb))
 * Vectorization/Tokenization
 * Stopword Removal
 * Other CountVectorizer options
 * Intro to [TextBlob](https://textblob.readthedocs.org/en/dev/)
 * Stemming and Lemmatization
* NLP Exercise [(notebook)](notebooks/13_NLP_rotten_tomatoes_exercise.ipynb)

**Homework:**
* **Your draft paper is due on Thursday (2/1)!** Please submit a link to your project repository (with paper, code, data, and visualizations) before class

**NLP Resources:**
* If you want to learn a lot more NLP, check out the excellent [video lectures](https://class.coursera.org/nlp/lecture) and [slides](http://web.stanford.edu/~jurafsky/NLPCourseraSlides.html) from this [Coursera course](https://www.coursera.org/course/nlp) (which is no longer being offered).
* This slide deck defines many of the [key NLP terms](https://github.com/ga-students/DAT_SF_9/blob/master/16_Text_Mining/DAT9_lec16_Text_Mining.pdf).
* [Natural Language Processing with Python](http://www.nltk.org/book/) is the most popular book for going in-depth with the [Natural Language Toolkit](http://www.nltk.org/) (NLTK).
* [A Smattering of NLP in Python](https://github.com/charlieg/A-Smattering-of-NLP-in-Python/blob/master/A%20Smattering%20of%20NLP%20in%20Python.ipynb) provides a nice overview of NLTK
* [spaCy](http://spacy.io/) is a newer Python library for text processing that is focused on performance (unlike NLTK).
* If you want to get serious about NLP, [Stanford CoreNLP](http://nlp.stanford.edu/software/corenlp.shtml) is a suite of tools (written in Java) that is highly regarded.
* When working with a large text corpus in scikit-learn, [HashingVectorizer](http://scikit-learn.org/stable/modules/feature_extraction.html#vectorizing-a-large-text-corpus-with-the-hashing-trick) is a useful alternative to CountVectorizer.
* [Automatically Categorizing Yelp Businesses](http://engineeringblog.yelp.com/2015/09/automatically-categorizing-yelp-businesses.html) discusses how Yelp uses NLP and scikit-learn to solve the problem of uncategorized businesses.
* [Modern Methods for Sentiment Analysis](http://districtdatalabs.silvrback.com/modern-methods-for-sentiment-analysis) shows how "word vectors" can be used for more accurate sentiment analysis.
* [Identifying Humorous Cartoon Captions](http://www.cs.huji.ac.il/~dshahaf/pHumor.pdf) is a readable paper about identifying funny captions submitted to the New Yorker Caption Contest.

-----
<a name="reduction"></a>
### Class 14: Dimensionality reduction
**By the end of this lesson you will be able to:**
* Apply TF-IDF to text (Natural language Processing)
* Reduce dimensions using Principle Compoment analysis (Dimensionality reduction)

**Topics/Highlights**

* Natural Language Processing continued ([notebook](notebooks/13_natural_language_processing.ipynb))
	* Term Frequency-Inverse Document Frequency (TF-IDF)
  	*  Using TF-IDF to Summarize a Yelp Review
  	*  Sentiment Analysis
  	*  NLP Exercise continued with TF-IDF [(notebook)](notebooks/13_NLP_rotten_tomatoes_exercise.ipynb)
* Dimensionality reduction
	* [slides](slides/14_dimensionality_reduction.pdf)
	* [notebook - iris dataset](notebooks/14_PCA_iris.ipynb)
	* [notebook - images dataset](notebooks/14_PCA_images.ipynb)

**NLP Resources:**
* If you want to learn a lot more NLP, check out the excellent [video lectures](https://class.coursera.org/nlp/lecture) and [slides](http://web.stanford.edu/~jurafsky/NLPCourseraSlides.html) from this [Coursera course](https://www.coursera.org/course/nlp) (which is no longer being offered).
* This slide deck defines many of the [key NLP terms](https://github.com/ga-students/DAT_SF_9/blob/master/16_Text_Mining/DAT9_lec16_Text_Mining.pdf).
* [Natural Language Processing with Python](http://www.nltk.org/book/) is the most popular book for going in-depth with the [Natural Language Toolkit](http://www.nltk.org/) (NLTK).
* [A Smattering of NLP in Python](https://github.com/charlieg/A-Smattering-of-NLP-in-Python/blob/master/A%20Smattering%20of%20NLP%20in%20Python.ipynb) provides a nice overview of NLTK
* [spaCy](http://spacy.io/) is a newer Python library for text processing that is focused on performance (unlike NLTK).
* If you want to get serious about NLP, [Stanford CoreNLP](http://nlp.stanford.edu/software/corenlp.shtml) is a suite of tools (written in Java) that is highly regarded.
* When working with a large text corpus in scikit-learn, [HashingVectorizer](http://scikit-learn.org/stable/modules/feature_extraction.html#vectorizing-a-large-text-corpus-with-the-hashing-trick) is a useful alternative to CountVectorizer.
* [Automatically Categorizing Yelp Businesses](http://engineeringblog.yelp.com/2015/09/automatically-categorizing-yelp-businesses.html) discusses how Yelp uses NLP and scikit-learn to solve the problem of uncategorized businesses.
* [Modern Methods for Sentiment Analysis](http://districtdatalabs.silvrback.com/modern-methods-for-sentiment-analysis) shows how "word vectors" can be used for more accurate sentiment analysis.
* [Identifying Humorous Cartoon Captions](http://www.cs.huji.ac.il/~dshahaf/pHumor.pdf) is a readable paper about identifying funny captions submitted to the New Yorker Caption Contest.

-----

<a name="decision"></a>
### Class 15: Decision Trees
**By the end of this lesson you will be able to:**

* Create a Regression tree
* Graph and interpret the decision tree

**Topics/Highlights**

* Decision trees ([notebook](notebooks/15_decision_trees.ipynb))
	* Part 1: Regression trees
* Exercise with Capital Bikeshare data ([notebook](notebooks/15_bikeshare_exercise.ipynb), [data](data/bikeshare.csv), [data dictionary](https://www.kaggle.com/c/bike-sharing-demand/data))

**Homework:**
* Read the "Wisdom of the crowds" section from MLWave's post on [Human Ensemble Learning](http://mlwave.com/human-ensemble-learning/).
* **Optional:** Read the abstract from [Do We Need Hundreds of Classifiers to Solve Real World Classification Problems?](http://jmlr.csail.mit.edu/papers/volume15/delgado14a/delgado14a.pdf), as well as Kaggle CTO Ben Hamner's [comment](https://news.ycombinator.com/item?id=8719723) about the paper, paying attention to the mentions of "Random Forests".

**Resources:**
* scikit-learn's documentation on [decision trees](http://scikit-learn.org/stable/modules/tree.html) includes a nice overview of trees as well as tips for proper usage.
* For a more thorough introduction to decision trees, read section 4.3 (23 pages) of [Introduction to Data Mining](http://www-users.cs.umn.edu/~kumar/dmbook/index.php). (Chapter 4 is available as a free download.)
* If you want to go deep into the different decision tree algorithms, this slide deck contains [A Brief History of Classification and Regression Trees](https://drive.google.com/file/d/0B-BKohKl-jUYQ3RpMEF0OGRUU3RHVGpHY203NFd3Z19Nc1ZF/view).
* [The Science of Singing Along](http://www.doc.gold.ac.uk/~mas03dm/papers/PawleyMullensiefen_Singalong_2012.pdf) contains a neat regression tree (page 136) for predicting the percentage of an audience at a music venue that will sing along to a pop song.
* Decision trees are common in the medical field for differential diagnosis, such as this classification tree for [identifying psychosis](http://www.psychcongress.com/sites/naccme.com/files/images/pcn/saundras/psychosis_decision_tree.pdf).

-----

<a name="ensemble"></a>
### Class 16: Ensembling, Bagging and Random Forests

* Decision trees ([notebook](notebooks/15_decision_trees.ipynb))
	* Part 2: Classification trees
* Ensembling, Bagging and Random Forests ([notebook](notebooks/16_ensembling.ipynb))
    * [Major League Baseball player data](data/hitters.csv) from 1986-87
    * [Data dictionary](https://cran.r-project.org/web/packages/ISLR/ISLR.pdf) (see page 7)

**Resources:**
* scikit-learn's documentation on [ensemble methods](http://scikit-learn.org/stable/modules/ensemble.html) covers both "averaging methods" (such as bagging and Random Forests) as well as "boosting methods" (such as AdaBoost and Gradient Tree Boosting).
* MLWave's [Kaggle Ensembling Guide](http://mlwave.com/kaggle-ensembling-guide/) is very thorough and shows the many different ways that ensembling can take place.
* Browse the excellent [solution paper](https://docs.google.com/viewer?url=https://raw.githubusercontent.com/ChenglongChen/Kaggle_CrowdFlower/master/Doc/Kaggle_CrowdFlower_ChenglongChen.pdf) from the winner of Kaggle's [CrowdFlower competition](https://www.kaggle.com/c/crowdflower-search-relevance) for an example of the work and insight required to win a Kaggle competition.
* [Interpretable vs Powerful Predictive Models: Why We Need Them Both](https://medium.com/@chris_bour/interpretable-vs-powerful-predictive-models-why-we-need-them-both-990340074979) is a short post on how the tactics useful in a Kaggle competition are not always useful in the real world.
* [Not Even the People Who Write Algorithms Really Know How They Work](http://www.theatlantic.com/technology/archive/2015/09/not-even-the-people-who-write-algorithms-really-know-how-they-work/406099/) argues that the decreased interpretability of state-of-the-art machine learning models has a negative impact on society.
* For an intuitive explanation of Random Forests, read Edwin Chen's answer to [How do random forests work in layman's terms?](http://www.quora.com/Random-Forests/How-do-random-forests-work-in-laymans-terms/answer/Edwin-Chen-1)
* [Large Scale Decision Forests: Lessons Learned](http://blog.siftscience.com/blog/2015/large-scale-decision-forests-lessons-learned) is an excellent post from Sift Science about their custom implementation of Random Forests.
* [Unboxing the Random Forest Classifier](http://nerds.airbnb.com/unboxing-the-random-forest-classifier/) describes a way to interpret the inner workings of Random Forests beyond just feature importances.
* [Understanding Random Forests: From Theory to Practice](http://arxiv.org/pdf/1407.7502v3.pdf) is an in-depth academic analysis of Random Forests, including details of its implementation in scikit-learn.

-----

<a name="time1"></a>
### Class 17: Modeling with Time Series Data I
**By the end of this lesson you will be able to:**

* Determine Timeseries data metrics using autocorrelation, rolling and expanding

**Topics/Highlights**
* Time series intro ([slides](https://docs.google.com/presentation/d/1pbAy7Pj-jZGFlcqkuiX8f-y7ozdiotBskkXaD5jiaKc/edit?usp=sharing))
* Exercises [(notebook)](notebooks/17_time_series_I.ipynb)

-----

<a name="time2"></a>
### Class 18: Modeling with Time Series Data II

* Time series intro ([slides](https://docs.google.com/presentation/d/12lBrOxtqhQRJ85PdkTr4qgcFy0DwUGzVy6bvdA5qyOs/edit?usp=sharing))
* Time series modeling with statsmodels [(notebook)](notebooks/18_timeseries_modeling.ipynb)
* Exercise with Wal-mart sales data [(notebook)](notebooks/18_Wal-mart_timeseries_exercise.ipynb)

-----

<a name="19_topics"></a>
### Class 19: Bonus Topics

**Topics/Highlights**

* Using a multi-user git repository - Exercise
<!-- * More uses for command line and BASH -->
* Review of what we have learned over the past 10 weeks

<!--
* Trends
	* Data storage, Hadoop and MapReduce
		* SQL databases
		* NoSQL vs. SQL databases ([comparison](http://core0.staticworld.net/images/article/2014/10/sql-nosql-b-100527236-large.idge.gif))
		* Distributed files [(diagram)](https://www.google.com/search?q=hadoop+storage+impala+diagram&source=lnms&tbm=isch)
	* AWS, Azure and Google,  data and data science engine services
		* SQL Databases in the cloud
			* AWS Redshift, Oracle, SQL Server
			* Azure SQL Server
			* Google BigQuery
		* NoSQL Databases
			* AWS Mongo, DynamoDB
			* Azure
		* Data collection for IoT
		* Data science software as a service (SaaS) engines - ex. [Azure Machine Learning](https://azure.microsoft.com/en-us/services/machine-learning/)
		* Machine learning with computer clusters: [Spark](http://spark.apache.org/) with [MLlib](http://spark.apache.org/mllib/)
-->

* Additional models and variants - Exercise  
* Data science software as a service (SaaS) engines - ex. [Azure Machine Learning](https://azure.microsoft.com/en-us/services/machine-learning/)
* Machine learning with computer clusters: [Spark](http://spark.apache.org/) with [MLlib](http://spark.apache.org/mllib/)
* Top takeaways and top surprises - Exercise [(form)](https://docs.google.com/forms/d/e/1FAIpQLSc837trmGghoDtx_wFsU6QJuESCp9D4TM3q9VuuSCWeo0WLQA/viewform)
* Where to go from here data scientists!
	* [Data science skills hierarchy](https://docs.google.com/spreadsheets/d/1RAcC44o3crC2ZeCmtrELibV1VyEB5ecnBHZKXXXZI6M)
* Next steps in your journey
	* [Exercise: your objectives and next steps](https://docs.google.com/spreadsheets/d/13z-eUjMtsSyO6B51iVzoEwmfpO-IhymoYDIVvgTious/edit?usp=sharing)

<!--
**Additional models and variants (in blue)**
* Classifiers
	* Naïve Bayes
	* KNN
	* SVC
	* [SDG](http://scikit-learn.org/stable/modules/sgd.html)
	* Decision Trees
	* Neural Networks
	* Ensemble methods [(scikit-learn pqge)](http://scikit-learn.org/stable/modules/classes.html#module-sklearn.ensemble)
		* Bagging
		* Boosting
			* [sklearn.ensemble.AdaBoostRegressor](http://scikit-learn.org/stable/modules/generated/sklearn.ensemble.AdaBoostRegressor.html)
			* Beware, even one misclassified label in training data can result in poor prediction
		* Random Forests
* Regression
	* Linear regression
	* [Ridge regression](http://scikit-learn.org/stable/modules/linear_model.html) 
	* [Lasso](http://scikit-learn.org/stable/modules/linear_model.html)
	* Logistic Regression
	* [Linear regressor with polynomial preprocessing](http://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.PolynomialFeatures.html)
	* [SVR (choose from several kernels)](http://scikit-learn.org/stable/auto_examples/svm/plot_svm_regression.html)
	* [SDG regression](http://scikit-learn.org/stable/modules/sgd.html)
	* Ensemble methods
		* [Random Forest regression](http://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestRegressor.html)
* Clustering
	* K-means
	* DBSCAN
	* [Hierarchical clustering](https://joyofdata.shinyapps.io/hclust-shiny/)
-->

-----

<a name="svc"></a>
### Bonus Content: Support Vector Classifier - SVC
* SVC (Support Vector Classifier)
 * [slides](slides/bonus_nn_svm.pdf)
 * [notebook](notebooks/bonus_nn_svc.ipynb)

**SVC resources**
* For a more in-depth inderstanding of Support Vector Machines and SVC, read Chapter 9 of Hastie and Tibshirani's excellent book, [An Introduction to Statistical Learning](http://www-bcf.usc.edu/~gareth/ISL/). (It's a free PDF download!)
* SVC videos by the authors of An Introduction to Statistical Learning can be found [here](http://www.dataschool.io/15-hours-of-expert-machine-learning-videos/).

-----

<a name="bayes"></a>
### Bonus content: Naive Bayes and Text Data
* Conditional probability and Bayes' theorem
    * [Slides](slides/bonus_bayes_theorem.pdf) (adapted from [Visualizing Bayes' theorem](http://oscarbonilla.com/2009/05/visualizing-bayes-theorem/))
    * Applying Bayes' theorem to iris classification ([notebook](notebooks/bonus_bayes_theorem_iris.ipynb))
* Naive Bayes classification
    * [Slides](slides/bonus_naive_bayes.pdf)
    * Spam filtering example ([notebook](notebooks/bonus_naive_bayes_spam.ipynb))
* Applying Naive Bayes to text data in scikit-learn ([notebook](notebooks/bonus_text_data_sklearn.ipynb))
    * [CountVectorizer](http://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.CountVectorizer.html) documentation
    * SMS messages: [data](data/sms.tsv), [data dictionary](https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection)

**Resources:**
* Sebastian Raschka's article on [Naive Bayes and Text Classification](http://sebastianraschka.com/Articles/2014_naive_bayes_1.html) covers the conceptual material from today's class in much more detail.
* For more on conditional probability, read these [slides](https://docs.google.com/presentation/d/1psUIyig6OxHQngGEHr3TMkCvhdLInnKnclQoNUr4G4U/edit#slide=id.gfc69f484_00), or read section 2.2 of the [OpenIntro Statistics textbook](https://www.openintro.org/stat/textbook.php?stat_book=os) (15 pages).
* For an intuitive explanation of Naive Bayes classification, read this post on [airport security](http://www.quora.com/In-laymans-terms-how-does-Naive-Bayes-work/answer/Konstantin-Tt).
* For more details on Naive Bayes classification, Wikipedia has two excellent articles ([Naive Bayes classifier](http://en.wikipedia.org/wiki/Naive_Bayes_classifier) and [Naive Bayes spam filtering](http://en.wikipedia.org/wiki/Naive_Bayes_spam_filtering)), and Cross Validated has a good [Q&A](http://stats.stackexchange.com/questions/21822/understanding-naive-bayes).
* When applying Naive Bayes classification to a dataset with continuous features, it is better to use [GaussianNB](http://scikit-learn.org/stable/modules/generated/sklearn.naive_bayes.GaussianNB.html) rather than [MultinomialNB](http://scikit-learn.org/stable/modules/generated/sklearn.naive_bayes.MultinomialNB.html). This [notebook](notebooks/bonus_types_of_naive_bayes.ipynb) compares their performances on such a dataset. Wikipedia has a short [description](https://en.wikipedia.org/wiki/Naive_Bayes_classifier#Gaussian_naive_Bayes) of Gaussian Naive Bayes, as well as an excellent [example](https://en.wikipedia.org/wiki/Naive_Bayes_classifier#Sex_classification) of its usage.
* These [slides](http://www.umiacs.umd.edu/~jbg/teaching/DATA_DIGGING/lecture_05.pdf) from the University of Maryland provide more mathematical details on both logistic regression and Naive Bayes, and also explain how Naive Bayes is actually a "special case" of logistic regression.
* Andrew Ng has a [paper](http://ai.stanford.edu/~ang/papers/nips01-discriminativegenerative.pdf) comparing the performance of logistic regression and Naive Bayes across a variety of datasets.
* If you enjoyed Paul Graham's article, you can read [his follow-up article](http://www.paulgraham.com/better.html) on how he improved his spam filter and this [related paper](http://www.merl.com/publications/docs/TR2004-091.pdf) about state-of-the-art spam filtering in 2004.
* Yelp has found that Naive Bayes is more effective than Mechanical Turks at [categorizing businesses](http://engineeringblog.yelp.com/2011/02/towards-building-a-high-quality-workforce-with-mechanical-turk.html).

-----

<a name="nn"></a>
### Bonus Content: Intro to Neural Networks
* Artificial Neural Networks (ANN)
 * [slides](slides/bonus_nn_svm.pdf)
 * [notebook](notebooks/bonus_nn_svc.ipynb)

**Neural Network resources**
* For a more background of on Artificial Neural Networks view this series.  It describes the logic behind ANN from a low level logic step by step point of view: 
 * Part 1 https://www.youtube.com/watch?v=bxe2T-V8XRs
 * Part 2 https://www.youtube.com/watch?v=UJwK6jAStmg
 * Part 3 https://www.youtube.com/watch?v=5u0jaA3qAGk
 * Part 4 https://www.youtube.com/watch?v=GlcnxUlrtek
 * Part 5 https://www.youtube.com/watch?v=pHMzNW8Agq4
 * Part 6 https://www.youtube.com/watch?v=9KM9Td6RVgQ
 * Part 7 https://www.youtube.com/watch?v=S4ZUwgesjS8
