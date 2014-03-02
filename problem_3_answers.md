Given your previous design critiques, your experience with the previous graph visualization implementation and the reading of the article cited below (Lee et al., 2006), answer the following questions:

1. Which graph-related tasks does an ideal GitHub Network Graph need to address?
	The ideal GitHub Network Graph needs to address the connectivty of the commits, branches, users and repositories over a period of time. It would have various functionality that allows for the user to play around with the network in ways that makes sense. 
		-The GitHub Graph should be able to display the Adjacencies of the nodes (in GitHub, commits). It should show, how many and how they are connected to each other.
		-It should also be able to show Common Connection. If given a certain node, the graph should display all the nodes that it is connected to. It's how the GitHub Graph shows which commits came befor/after on a branch or when it was merged with another branch.

2. Get back to the GitHub network visualization you implemented and test it with the following projects on GitHub: D3, jQuery and Bootstrap. There's a lot more data, but the interaction patterns of users are also very different. What do you notice about the three repositories?
	
	D3: All of the activity seems to revolve around Mike Bonstock. All of the users merge with Mike Bonstock, whereas in the Calyedo all of the users merge with each other and they're working together.
	jQuery: There are a few people who's work seems to get merged with and they have many of the most recent commits, so either they've been working on the project the most recently. 
	Bootstrap: There are a few people working heavily on the project and committing and merging with each other, but there are a few who only interact once or twice. 

3. How does this impact your graph?
	It impacts the graph by making it much busier with lines overlapping and many more commits on top of one another. 

4. How would you improve your visualization to address issues with the larger and more complex data?
	I would turn it vertically in order to be able allow for more data to load and be more spaced out. Also, I would allow for the nodes to change sizes based on the commit (additions and deletions), so its much easier to differentiate between substantial commits and those with minor changes. 



Sketch an alternative to the GitHub Network Graph Visualizer

 The graph that I desgined has commits listed by in order that they were created by time from left to right. The nodes are different sizes (which are determined by a scale which varies value depending on the number of the additions and deletions made that week). When the user mouses over the node more information such as commit message and user and date come up. 

 I think that my new network shown in designstudio.jpg addresses the issues of determining quickly when a lot of work was done and when it wasn't.A commit doesn't always correlate with a lot of changes happing. By looking at this graph it is easy to quickly determine what weeks new features may have implemented and what weeks there may have not been that much work done. 
