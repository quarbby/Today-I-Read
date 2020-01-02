# Polarization, Partisanship and Junk News Consumption on Social Media During the 2018 US Midterm Elections

*Authors*: Nahema Marchal, Lisa-Maria Neudert, Bence Kollanyi, Philip N. Howard of Oxford Internet Institute

Link: http://blogs.oii.ox.ac.uk/comprop/wp-content/uploads/sites/93/2018/11/marchal_et_al.pdf

Year: Nov 2018

*Overview*

Examine sources of political news and information shared by social media users in the period leading up to the 2018 US midterms, evaluate sources and identify primary audiences for content that is sensational, extremist, conspiratorial or has other qualities of junk news

Research questions:
- What kinds of political news and information are social media users in the United States sharing in advance of Election Day?
- How much of it is extremist, sensationalist, conspiratorial, masked commentary, fake, or some other form of junk news?
- Which groups of voters in the US are sharing the highest amount of junk news and information?

*Corpus Construction*

- Analyse 2.5mil tweets and 6986 Facebook pages over a 30 day period

- Extracted URL links from 2.5mil tweets from 379k unique users collected during the lead up to US midterm election using a combination of relevant political party hashtags, election-specific hashtags and handles for individual parties. Hashtags were curated by Subject Matter Experts.
- Twitter Streaming API was used to collect publicly available tweets from hashtags. Tweets collected were:
 - contained at least one of the relevant hashtags or at least one Twitter handle of the political parties or political leader
 - contained the hashtag in the URL shared, or the title of its webpage
 - were a retweet of a message that contained a relevant hashtag or mention in the original message
 - were a quoted tweet referring to a tweet with a relevant hashtag or mention

- Team classified content in terms of: extremist, sensationalist, conspiratorial, masked commentary, fake news and other forms of junk news. Further elaboration of each is in the paper.

- Perform Facebook Network Mapping to search how URLs of these websites were being shared over Facebook
- Visualised social network data to understand how people share information and associate with each other
- Calculated heterophily score for each combination of group pairings to find combinations between two groups

*Conclusion*
- Amount of junk news in circulation over social media is greater than 2016 US presidential election, with users sharing more junk news than professional news overall
- Junk news once consumed by PResident Trump's support base and the far-right is now consumed by more maintream conservative social media users
- Less than 5% of the sources referenced on social media are from public agencies, experts or political candidates themselves.


*Other Notes*
- [Notes Link](https://comprop.oii.ox.ac.uk/wp-content/uploads/sites/93/2018/11/midterms_supplement.pdf)
- Construction og graph visualisation with the Fruchterman-Reingold algorithm
- Understanding ties between two groups using the Heterophily Index. A greater heterophily index indicates a denser pattern of connections between the two groups. This score indicate only first order connections, not second or third.
- Clustering algorithm by building a bipartite graph between nodes in the map and the rest of the social medium in question. This bipartite graph provides a structural similarity metric between nodes in the map. This was then used in combination with a hierarchical agglomerative clustering algorithm in order to cluster a map into distinct communities. This is a ‘bottom up’ approach whereby each observation starts in its own cluster, and pairs of clusters are merged as one moves up the hierarchy. ([Related Paper](http://snap.stanford.edu/class/cs224w-2016/projects/cs224w-83-final.pdf)


