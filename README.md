Download Link: https://assignmentchef.com/product/solved-cisc5950-project-1-k-means
<br>
<span class="kksr-muted">Rate this product</span>

In this project, we are going to design our own Hadoop MapReduce-based program to analyze the data. The project consist of two parts.

NY Parking Violations

The NYC Department of Finance collects data on every parking ticket issued in NYC ( 10M per year!). This data is made publicly available to aid in ticket resolution and to guide policy- makers.

You can find the data from the Link of NYC Parking Data.

The above figure shows several records, where each row represents a parking ticket and the columns are the details of the tickets.

To start the project, you have to, 1. Start the 3-node cluster2. Set up the HDFS3. Store the data in HDFS

1

CISC 5950, Spring 2022 Big Data Programming

4. Set up the MapReduce framework along with the scheduler for resource management. By analyzing the data, we need to answer the following,

• When are tickets most likely to be issued?• What are the most common years and types of cars to be ticketed? • Where are tickets most commonly issued?• Which color of the vehicle is most likely to get a ticket?

NBA Shot Logs

https://www.kaggle.com/dansbecker/nba-shot-logs

This is the DATA (https://www.kaggle.com/dansbecker/nba-shot-logs ) on shots taken during the 2014-2015 season, who took the shot, where on the floor was the shot taken from, who was the nearest defender, how far away was the nearest defender, time on the shot clock, and much more. The column titles are generally self-explanatory.

The above figure shows several records, where each row represents a shot and the columns are the details of the shot, e.g. the game ID, who is the defender, what is the distance between them.

By analyzing the data, we need to answer the following,• For each pair of the players (A, B), we define the fear sore of A when facing B is the hit

rate, such that B is closet defender when A is shoting. Based on the fear sore, for each 2




player, please find out who is his ”most unwanted defender”.• For each player, we define the comfortable zone of shooting is a matrix of,

{SHOT DIST, CLOSE DEF DIST, SHOT CLOCK}

Please develop a MapReduce-based algorithm to classify each player’s records into 4 comfortable zones. Considering the hit rate, which zone is the best for James Harden, Chris Paul, Stephen Curry and Lebron James.

Bonus Question

The biggest challenge when using K-Means is to decide on the number of clusters. Having more clusters creates some small classes with very few records, while having less clusters leads to classes that are too general.

Based on a K-Means algorithm above, try to answer the following question,

<ul>

 <li>Given a Black vehicle parking illegally at 34510, 10030, 34050 (street codes). What is the probability that it will get an ticket? (very rough prediction).</li>

 <li>At 10 am, I want to go to Lincoln Center and I just want to walk within 0.5 mile. Where should I park? (Divided into zones).</li>