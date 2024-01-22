# DIME-Network-Analysis

[DIME](https://data.stanford.edu/dime) (Database on Ideology, Money in Politics, and Elections) is a data created and maintained by [Adam Bonica](https://web.stanford.edu/~bonica/), which entails monetary contributions in US Political Elections. In this study we focus on US Federal Elections and try to formulate an analysis to understand the underlying network, and its properties and showcase how we can create a community structure based on the different ideologies among the contributors/recipients. This study is the term project for the Network Science course (PHYS5116) at Northeastern University, which I took in Fall'23 under the guidance of [Prof. Albert Laszlo Barabasi](https://en.wikipedia.org/wiki/Albert-L%C3%A1szl%C3%B3_Barab%C3%A1si). 

# Network Visualization 

<img src="DIme Network 2012 Elections.png" alt="Federal Elections '12">

# Data and Preparations

As we can expect the contributions were in millions, and over the years kept on increasing. The data is very comprehensive and spans over a wide range of years starting from 1979 to 2020. Acknowledging the size, and computational limitations we worked with 2008 and 2012 election data, where we formulate a network as Contributors/Recipients being the nodes, and the transaction in between them being the edges (We dealt with ~16-20GB, leveraging high RAM machines, and sqlite3 database for processing). 

To formulate the network we did a lot of basic preprocessing steps like - 
- Matching similar Contributors and Recipient IDs (Using a Dictionary provided by Bonica),
- Summing contributions between the same nodes

We also faced many anomalies in the data which is further discussed along with other findings in the [deck attached](/DIME%20Final%20Report.pdf)

# Objective (High level)

There were a couple of objectives that we wanted to achieve with this study - 
1) Portray the underlying network in the Monetary Contributions - Showcase the scale-free properties, and prove that it's not a random network
2) Study the effect of [Citizens United Act '10](https://campaignlegal.org/update/how-does-citizens-united-decision-still-affect-us-2024) on Federal Elections

We successfully formulated both objectives and showcased the underlying network with an ideology-based community structure. 

