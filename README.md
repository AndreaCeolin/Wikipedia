# Wikipedia

If we want to study user interactions online, a good starting point would be collecting a large number of interactions that follow this scheme:

    UserA: post
    UserB: reaction to post
    UserA: reaction to B's reaction

If we run a sentiment analysis, it will be clear whether A is happier or not after B's comment. 

Here we collect a list of triplets of this kind using the [Wikipedia Talk Corpus](https://figshare.com/articles/Wikipedia_Talk_Corpus/4264973). This corpus contains the history of the comments made by users on Wikipedia articles from 2001 to 2015. 

First, download all the comments_articles_year folders on a 'wikimedia' folder. Then, download ```wiki_crawler.py``` in the same place.

If you run ```wiki_crawler.py```, the program will start extracting A-B-A triplets. The name of the folders which are explored are printed. Once the run is completed, you will have a file called ```filtered_wiki.tsv``` in the workspace with the following format:

    Time UserA1 Topic Comment
    Time UserB1 Topic Comment
    Time UserA1 Topic Comment
    Time UserA2 Topic Comment
    Time UserB2 Topic Comment
    Time UserA2 Topic Comment
    Time UserA3 Topic Comment
    ....
  
The file will contain a total of 167680 triplets. Now you can run your analysis.
Enjoy it!

  
  

