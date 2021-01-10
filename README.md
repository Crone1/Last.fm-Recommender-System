The project was done by myself and GitHub user *'adampower48'* as part of the module *'Advanced Machine Learning'*. The purpose of this project was to create a recommender system to recommend song artists to a user using the Last.fm dataset.

We combined this data with data we scraped from the Spotify API to get additional artist information.

To complete this task then, we took a few different approaches, developing three different systems. These systems used clustering, collaborative filtering and deep learning respectively.

The code for completing this recommendation task was then done using google collab for collaboration purposes and to get experiance using this platform. Afterwards, I coppied the developed code into this GitHub repository.
This code broke down into five different notebooks:

1.  The first notebook is the 'Data Processing' notebook.
    - This is where we read in the original data and combine it with some external data to ensure get all of the data in the one table.
    - This notebook exports a csv file containing a dataframe of all of the data we will use in this projct to make recommendations.

2.  After the data is processed, we bring it into the 'Data Exploration' notebook.
    - This is where we explore the data and gain a better understanding of what it contains.
    - This notebook does not export anything but is used for the sole purpose of giving us a better insights as to the contents of the data so that we can best utilise it for our recommendations.
    
3.  After processing the data in the 'Data Processing' notebook and exploring it in the 'Data Exploration' notebook, we now move on to the recommendation part of this project.
    - The first recommendation notebook to look at is the most basic recommender type and revolves around clustering.
    - This is contained in the 'Clustering Recommendation' notebook.
    - We wanted to incorporate some of the work we did in the *'Clustering-Decision-Data'* repositroy (https://github.com/Crone1/Clustering-decision-data) so this is where we do that.
    - This notebook is broken down into 7 parts, these are:
        1.   Reading in the processed data
        2.   Experimenting with the number of clusters
        3.   Clustering the users based on the artists and ratings
        4.   Create a vector for each cluster
        5.   Get the user input
        6.   Get a recommendation for this user
        7.   Output the recommendation
        
4.  The next recommender system that we built is a step up from the clustering, and uses a collaborative filtering approach. 
    - This is done in the 'Collaborative Filtering' notebook.
    - There is a simple interactive demo at the end of this notebook to show how the system can be used to generate recommendations for an existing user.
        - Note that you will need to run through the full notebook to build the system before the demo.
    - The notebook is split into five parts:
        1.  Setup & data loading
        2.  Creating user and artist embeddings
        3.  Matrix factorisation (i.e. training the model)
        4.  Generating recommendations (and demo)
        5.  Visualising the embeddings
        
5.  Finally, we look at a more complicated but flexible recommender system based on a deep learning approach.
    - This is done in the "Softmax Model" notebook.
    - There is a more comprehensive demo for this model which is much more like an end-user experience.
         - To run this you will need to first execute the rest of the notebook (except the model training part if you have access to the saved model weights).
    - There are four parts in this notebook:
        1.  Setup & data loading
        2.  Building & training the model
        3.  Building the user interface
        4.  Demo
    
