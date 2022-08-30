# PyPoll_Challenge: Analysis of the Election Audit

## Overview of Project

A Colorado Board of Elections employee, Tom,  has given the following tasks to be completed for the election audit of a recent local congressional election. Tom’s supervisor, Seth, would like these tasks done using Python, Visual Studio Code (VS Code)and store the audit and analysis in a GitHub Repository. Tom is providing the assistance to help the process along with download advice and training. The tasks are as follows:

•	Calculate the total number of votes cast.

•	Get a complete list of candidates who received votes.

•	Calculate the total number of votes each candidate received.

•	Calculate the percentage of votes each candidate won.

•	Determine the winner of the election based on popular vote.

•	Determine the votes by county for the congressional district including vote count and percent of total.

•	Determine which county has the highest vote turnout

## Resources
The resources were provided by the Elections employee Tom and Seth and included:

•	Data Source: election_results.csv

•	Software: Python 3.7.6, Visual Studio 1.70.2.

•	Instruction on how to use Python, VS Code and GitHub.



## Summary

### The Analysis of the Election show that:

•	There were 369,711 votes cast in the election. The votes by County were:
	
	o	Jefferson County with 10.5% of the votes and 38,855 votes.

	o	Denver County with 82.8% of the votes and 306,055 votes.

	o	Arapahoe County with 6.7% of the votes and 24,801 votes.


•	The candidates were:

	o	Charles Casper Stockham

	o	Diana DeGette

	o	Raymon Anthony Doane


### The Analysis of the election results were:
 
•	Charles Casper Stockham received 23% of the vote and 85,213 votes.

•	Diana DeGette received 73.8% of the vote and 272,892 votes.


•	Raymon Anthony Doane received 3.1% of the vote and 11,606 votes.


### The winner of the election was Diana DeGette who received 73.8% of the votes and 272,892 votes.

## Challenge Overview – creating the script.

•	We begin by adding our dependencies and adding a variable to load a file from a path. The CSV module and OS package are loaded so we can use the CSV data and work with our operating system then the variables are created (file_to_load) and (file_to_save) so we can access the data in the designated path and save the file to a designated path:

![	 ](https://github.com/Johnnytoobadman/Election_Analysis/blob/main/Analysis/Script01.png)

•	Next we initialize the vote counter and create lists and dictionaries for candidate options, candidate votes, County Names and County votes.  We will also establish variables for winning candidates, winning counts, winning percentage, Largest County turnout name and Largest County vote count:

![	 ](https://github.com/Johnnytoobadman/Election_Analysis/blob/main/Analysis/Script02.png)
 
•	Next we read the CSV file, convert it into a list of dictionaries and read the header row:

 ![](https://github.com/Johnnytoobadman/Election_Analysis/blob/main/Analysis/Script03.png)
	 

•	Then we start looping through each row in the dataset to count votes by county and candidate:
 
![	 ](https://github.com/Johnnytoobadman/Election_Analysis/blob/main/Analysis/Script04.png) 

•	We then determine using an ‘if” conditional if the candidate does not match an existing candidate (then add it to the list of candidate names).  Similarly we write an if statement that checks if the County does not match any counties in the list:
 
![	 ](https://github.com/Johnnytoobadman/Election_Analysis/blob/main/Analysis/Script05.png) 

•	We then establish the file save instructions, print the final total vote count to terminal and written to file as election results:
 
![	 ](https://github.com/Johnnytoobadman/Election_Analysis/blob/main/Analysis/Script06.png) 

•	Next we write a for loop to get the county from the county dictionary, retrieve the County vote count, get the county percentage of votes by county and print the county results to the terminal.  Nested in the “for loop” is a conditional statement that uses an if statement to determine the county name with the most votes which is then printed and written to file:

![	 ](https://github.com/Johnnytoobadman/Election_Analysis/blob/main/Analysis/Script07.png)
 
•	Similarly this same method of nesting a conditional in a for loop is used to determine the candidate name and vote count including the winning candidate by vote count and percentage. Again this last step is printed to the terminal and written to the text file as election results:

![	 ](https://github.com/Johnnytoobadman/Election_Analysis/blob/main/Analysis/Script08.png)

## Challenge summary

•	Python coding is very powerful but requires a lot of preparation, knowledge and planning to write the script accurately.
  
•	Visual Studio Code was instrumental is identifying syntax errors, indent errors and more in the long process of working through this project.

•	Writing the conditional statements to determine the winning candidate and County by votes and percentages was extremely challenging.
