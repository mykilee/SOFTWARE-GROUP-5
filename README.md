# mcu-social-network-analysis
A social network analysis performed on the Marvel Cinematic Universe. By creating a dataset via web scraping, I was able to measure the structural properties of the network and create data visualizations using Gephi.


# Background & Desciption
- The objective is to gather a holistic understanding of the MCU network and analyze how it is connected, explore which components are essential to its unity and the communities that exist within. 
- Prior datasets were predominately focused on the comic series or a limited MCU (movies) list. I chose to create my own dataset to ensure that it contained proper and updated information. 
- I utilized the Internet Movie Database (IMDb) as a reliable source to collect the information for my dataset. I chose to select 40-70 main actors from each film to ensure that redundancies were limited, and only primary characters were gathered. To easily filter out the background characters, I pulled only the “credited” actors from the IMDb list. Credited versus uncredited actors were indicated on the webpage and within the HTML to create for a faster/more efficient collection. 
- With the Gephi software, I was able to perform analyses to calculate the structural properties of the network and create multiple data visualizations to get a graphical understanding of how the network interacts. I conducted several centrality measures on the dataset to get a diverse understanding of its structure. Techniques that I implemented were calculating density, modularity (community/subgroups), betweenness, and closeness. 

# Technologies Used 
- Python -- web scraping program
- Gephi -- data visualization software

# Background Knowledge
- Betweenness centrality is the interaction between two non-adjacent actors relying on the other actors lying on the paths between them. A high betweenness centrality indicates a node that is best for connecting different subgroups/nodes across the network. It is calculated by CB (ni) = ∑j<k ( gjk (ni ) / gjk ). 
- Closeness centrality is a similar measure that demonstrates how close an actor is to the others. This indicates how quickly a node can communicate or interact with the rest of the network. Closeness centrality = Cc (ni) = 1 /  (g∑i = 1 d( ni, nj )), as the higher the result, the greater the importance the node holds in the graph. These provided multiple viewpoints to demonstrate how it is linked with one another, which characters act as a bridge connecting nodes, and other indicators to find the most important actors.

# Tips for Gephi Use
- If you download this repository and want to interact with the data visualizations/Gephi software, these are some tips for analyses and statistics that you can apply: 
  - On the LHS, the "Layout" section allows you to apply various algorithms to display the dataset. 2 that I used and found most beneficial in visualizing the network are Force Atlas and Fruchterman Reingold. 
  - On the RHS, the "Statistics" section is where you can apply structural property measurements and other various SNA methodologies. I found it valuable to compute the Average Degree, Network Diameter, and Modularity. Primarily "Network Diameter" has multiple statistics included: Betweenness Centrality, Closeness Centrality, and Eccentricity. Once these computations are done, more visualization tools are made available. 
  
- Once the Statistics are computed, you can apply various techniques for your data vis.
  -  In Force Atlas, I changed "Repulsion Strength" to 1000.0 and selected the "Adjust by Sizes" option.  
  -  With Fruchterman Reingold, I left the preset numbers and "Run" the algorithm until there is a stable, circular/globe-like shape. 
  
- Regardless of algorithm applied, the below is relative to both:  
  - Appearance (Top LHS) > Nodes > Partition > Modularity  -->  this displays community detection
  - Appearance > Nodes > Ranking > Betweenness, Closeness, Eccentricity, and Modularity (and more) are available --> this is also helpful in visualizing the network based on the statistics. 

# Another Tip/Learning Resource
- https://www.youtube.com/watch?v=371n3Ye9vVo
- I found her tutorial helpful, explanatory, and to the point with understanding what certain tools do. 

# P.S. 
- Although the MCU is a fictional network, this approach and the applied methodologies pertain to how real-life SNA can be employed. 
- Hopefully other Marvel fans alike enjoy!  
