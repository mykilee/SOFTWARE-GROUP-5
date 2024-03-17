# mcu-social-network-analysis
A social network analysis performed on the Marvel Cinematic Universe(MCU). By creating a dataset via web scraping(IMDb), we were able to measure the structural properties of the network and create data visualizations using Gephi.


# Background & Desciption
- The objective is to gather a holistic understanding of the MCU network and analyze how it is connected, explore which components are essential to its unity and the communities that exist within. 
- Prior datasets were predominately focused on the comic series or a limited MCU (movies) list. We chose to create dataset to ensure that it contained proper and updated information. 
- We utilized the Internet Movie Database (IMDb) as a reliable source to collect the information for our dataset. We chose to select 40-70 main actors from each film to ensure that redundancies were limited, and only primary characters were gathered. To easily filter out the background characters, We pulled only the “credited” actors from the IMDb list. 
- With the Gephi software, we were able to perform analyses to calculate the structural properties of the network and create multiple data visualizations to get a graphical understanding of how the network interacts. We conducted several centrality measures on the dataset to get a diverse understanding of its structure. Techniques that we implemented were calculating density, modularity (community/subgroups), betweenness, and closeness. 

# Technologies Used 
- Python for web scraping
- Gephi for data visualization

# Background Knowledge
- Betweenness centrality is the interaction between two non-adjacent actors relying on the other actors lying on the paths between them. A high betweenness centrality indicates a node that is best for connecting different subgroups/nodes across the network. It is calculated by CB (ni) = ∑j<k ( gjk (ni ) / gjk ). 
- Closeness centrality is a similar measure that demonstrates how close an actor is to the others. This indicates how quickly a node can communicate or interact with the rest of the network. Closeness centrality = Cc (ni) = 1 /  (g∑i = 1 d( ni, nj )), as the higher the result, the greater the importance the node holds in the graph. These provided multiple viewpoints to demonstrate how it is linked with one another, which characters act as a bridge connecting nodes, and other indicators to find the most important actors.

# Limitations
- Data volume: due to the large number of characters in the movies, collecting all relevant characters may be very time-consuming and labor-intensive. Therefore, we may only be able to select certain characters or movies for analysis, which may result in limitations and incompleteness of the network.
- Lack of contextual information: relying solely on the frequency of appearances or co-occurrences between characters may not fully understand the relationships between characters, lack of background information may limit a deeper understanding of interactions between characters.
- Data reliability, although we can obtain data from sources such as IMDb, these data may contain errors or be incomplete. Some characters may be missed or not listed correctly, which may affect the accuracy of network analysis.

# Solutions
- Combining multiple data sources, such as IMDb, Marvel official materials, and other online databases, the accuracy and completeness of the data can be improved.
- Extension of social network theory: considering the use of more complex social network theories and models, such as dynamic network analysis or heterogeneous network analysis, to better simulate the complex relationships between characters in Marvel movies.

# Reference
Ahnert, R., Ahnert, S. E., Coleman, C. N., & Weingart, S. B. (2020). The network turn: Changing perspectives in the humanities. Cambridge University Press.
