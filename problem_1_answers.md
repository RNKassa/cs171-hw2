For each of the 5 visualizations listed above plus the calendar map, answer the following questions:

1. Who is the audience? (e.g. project manager, contributor, project user, visitor, etc.)

Contributors to a repository: The project manager, contributors, visitor (intersted in knowing who made the code in the project)
Commits Activity: The project manager, visitor (to see how recently the code was made and changed)
Code Frequency: The project manager and visitors 
Punch Card: The project manager and contributors
Pulse of a Repository: Project Manager and contributors and curious vistors



2. What data have been used? How can you get the data using the GitHub API? (Note that it can be the combination of multiple queries and their processing).

The data used in each of the visualizations can be found in using the following parts of the GitHub APIs.

Contributors to a repository: https://api.github.com/repos/Caleydo/caleydo/contributors

Commits Activity: https://api.github.com/repos/Caleydo/caleydo/commits

Code Frequency: https://api.github.com/repos/Caleydo/caleydo/stats/code_frequency

Punch Card: https://api.github.com/repos/Caleydo/caleydo/stats/punch_card

Pulse of a Repository:  https://api.github.com/repos/Caleydo/caleydo/pulls
						https://api.github.com/repos/Caleydo/caleydo/pulls/:number/merge
						https://api.github.com/repos/Caleydo/caleydo/stats/contributors
						https://api.github.com/repos/Caleydo/caleydo/commits
						https://api.github.com/repos/Caleydo/caleydo/issues/comments

						

3. Those visualizations are updated over time. What happens if suddenly a contributor pushes many commits in a short time interval? How would you address this particular issue?
Contributors to a repository: The graph will adjust with just a high peak corresponding to the peak in commits 
Code Frequency: Like the "contributors to a repository" graph there would be a spike in the peak in commits
Punch Card: The scale of the size of the circles would have to adjust in order to be able to handle an high peak. Or just have a max size so it doesn't mess up the rest of the visualization
Pulse of a Repository: No affect on this.


4. Looking at the network graph:


	Who is the audience? (e.g. project manager, contributor, project user, visitor, etc.)
		The audience is the contributors and project manager to observe progress on the project. 

	What data have been used? How can you get the data using the GitHub API? (Note that it can be the combination of multiple queries and their processing)
						
						https://api.github.com/repos/Caleydo/caleydo/pulls
						https://api.github.com/repos/Caleydo/caleydo/pulls/:number/merge
						https://api.github.com/repos/Caleydo/caleydo/stats/contributors
						https://api.github.com/repos/Caleydo/caleydo/commits

	Those visualizations are updated over time. What happens if suddenly a contributor pushes many commits in a short time interval? How would you address this particular issue?
		There will be a bunch of dots on the branch or master. If need be the dots can be over lapped and enlarged (to signify more commits over a small period of time). 

	What is the role of interaction for this visualization? Would a static graph have been sufficient?
		The role of the interaction for this visualization is to enable the viewer to see how the repository has been interacted with over the course of time. No the a static graph would not have been sufficient because if the repository has been around for more than a few days much of the information the graph offers is cut out.

	What happens if many new developers suddenly join the project and push commits for the first time? How would you preserve the graph's readability in such a situation?
		You can simplify the graph by stacking the lines that are formed from the join and pushing of commits at the same time. 


Over the course of the pset I used the following websites for help:
http://chimera.labs.oreilly.com/books/1230000000345/ch10.html#_html_div_tooltips
http://alignedleft.com/tutorials/d3/axes
https://leanpub.com/D3-Tips-and-Tricks/read

















