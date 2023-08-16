# BC-Project-1_Group-8 
Project Title: Impacts on Home Pricing
Data Visualization & Analytics: Project-1 Group-8
By: Angela Gosewehr, Naseema Omer, Noah McHale, &  Tristan Vazquez
Special Thank you to our Instructor and TAs: Hunter Hollis, Sam Espe, & Randy.

# Getting started 
Github repository created and cloned 'https://github.com/NMcHale029/BC-Project-1'
Github repository for Jupyter Notebook scripts and output files

Google Docs folder created: https://drive.google.com/drive/folders/119aAy9vImAUEnMLyTJ8geEU1sqUHDeBJ?usp=drive_link
Google docs for Project Proposal doc, Presentation slides

# Dataset selection 
Selection criteria:
	Public, Free, reliable, with Usability rate of 10
    File Type: CSV 
    Size: sufficient workable data
Selected Dataset:	
‘USA Real Estate Datatest’ available on Kaggle.com 
https://www.kaggle.com/datasets/ahmedshahriarsakib/usa-real-estate-dataset

# Add your files
Dataset csv file 'realtor_data.csv', gitignore, README.md

# Integrate with your tools
Each team member cloned the repository
Jupyter Notebooks for scripts

# Test and Deploy
Each team member tested access to repository with push and pull 
Will sync/ upload/ merge final scripts

# Project Description
Identify any correlation of certain residential home traits on House Pricing within USA States using a real estate data set. 

# Analysis
Research 3 main questions included in the approved Project Proposal: 
1. Q1: What impact do the number of bedrooms, number of bathrooms, acreage and house size have on House Sale Prices of four selected States?   What has the strongest correlation?
2. Q2: How do the above correlations vary by State?
3. Q3: What is the average pricing for a 3 bedroom, 2 bathroom home by State? 	

# Steps & Analysis 
1. Clean the input source realtor_data.csv data and create the clean_states.csv that is used for the other scripts in this project. 
script: data_cleaning.ipynb 

4 selected States based upon amount of data present in the file: Connecticut, Massachusetts, New Jersey, New York. 

Remove null, outliers. Retain the needed columns for 4 States used in study: Connecticut, Massachusetts, New Jersey, and New York
Assumptions: Duplicates may be present on the criteria of 'sold date' and 'address' 

2. Q1 and Q2 Analysis and Visualization
Script: 'variable_analysis.ipynb'

Process: 
Create new data frames for each state by filtering our original data frame. Create scatter plots to display each independent variable in relation to house price. Run linear regression for each plot and calculate the squared r-value for each variable to determine how much of the variation of the home price is explained by our independent variables.

Steps:
Create new data frames to only include relevant state.
Use created  function to: 
-populate scatter plots
-calculate correlation 
-run linear regression
-display linear regression equation
Call each independent variable in function to create desired plot and display R-squared for each state.

3. Q3 Analysis and Visualization script '
Script: 

4. Add-On / not in the Project Proposal: 
Q4: a. Identify the median and standard deviation for all 4 states on Price, Bedrooms, Bathrooms, Acreage and Size 
b. what is the average price in cities for State of NY. Selected NY as it had the highest STD in Price. 

Analysis 4a: Mean, STD, ran successfully for all 4 States on Home Prices, Number of Bedrooms, Number of Bathrooms, Acreage, and Size.  
Findings: Average Price and Standard Deviation (STD) for each State reveals:
1. NY with the highest STD for Price in comparison with Connecticut, Massachusettes, and New Jersey. 
2. The Median Number of Bedroom and Bathroom values reveal the average is 3 Bedrooms, and 2 Bathrooms. Identified that the average mean of a home in all four states is of 3 Bedrooms and 2 Bathrooms. 

4b. Used source file from kaggle.com called UnitedStates Cities DB 'uscities.csv' to get coordinates: Latitude and Longitude for each city in State of New York. 
Identified that 106 of the 274 cities for NY State in this project had coordinates in the uscities.csv file. 
suspended looking further into this question. 
future study that may be more beneficial would be perhaps to study the increase in the average price of each city for one or more States over a period of time. Could utilize the sold date and address of the house. 
 

# Visuals 
PASTE SCREEN SHOTS HERE from Q1, Q2 and Q3 plots here. 
? Depending on what you are making, it can be a good idea to include screenshots or even a video (you'll frequently see GIFs rather than actual videos). Tools like ttygif can help, but check out Asciinema for a more sophisticated method.

# Installation
? Within a particular ecosystem, there may be a common way of installing things, such as using Yarn, NuGet, or Homebrew. However, consider the possibility that whoever is reading your README is a novice and would like more guidance. Listing specific steps helps remove ambiguity and gets people to using your project as quickly as possible. If it only runs in a specific context like a particular programming language version or operating system or has dependencies that have to be installed manually, also add a Requirements subsection.

## Usage
Use examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.

# Support
? Tell people where they can go to for help. It can be any combination of an issue tracker, a chat room, an email address, etc.

# Roadmap
Frequency of releases / updates to this project by initial team: Never.

# Contributing
?State if you are open to contributions and what your requirements are for accepting them.

For people who want to make changes to your project, it's helpful to have some documentation on how to get started. Perhaps there is a script that they should run or some environment variables that they need to set. Make these steps explicit. These instructions could also be useful to your future self.

You can also document commands to lint the code or run tests. These steps help to ensure high code quality and reduce the likelihood that the changes inadvertently break something. Having instructions for running tests is especially helpful if it requires external setup, such as starting a Selenium server for testing in a browser.

# License
open source / no licensure required

# Project status
?If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.

