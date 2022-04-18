# Election_Analysis

## Project Overview

This project was meant to audit the results of a U.S. Congressional precinct in Colorado. The aim of the audit was to help provide data on how many votes each candidate received and to help determine which county had the highest voter turnout. Voter data was imported from a 'CSV' and then each row was iterated over to obtain voter data. 


1. Calculate the total number of votes cast
2. Get a complete list of candidates who received votes
3. Calculate the total number of votes each candidate received
4. Calculate the percentage of votes each candidate won
5. Determine the winner of the election based on popular vote

## Resources
- Data source: election_results.csv
- software: Python 3.7.6 Visual Studio Code 1.64

## Election Audit Results

=======
## Summary
Analysis of election shows that


Election Results
-------------------------
* Total Votes: 369,711

* Jefferson: 10.5% (38,855)
* Denver: 82.8% (306,055)
* Arapahoe: 6.7% (24,801)
* Largest County Turnout: Denver
-------------------------
* Charles Casper Stockham: 23.0% (85,213)
* Diana DeGette: 73.8% (272,892)
* Raymon Anthony Doane: 3.1% (11,606)
-------------------------
* Winner: Diana DeGette
* Winning Vote Count: 272,892
* Winning Percentage: 73.8%

![Results](/Resources/results2.PNG)

## Election Audit Summary
This code is designed to be run with voter data in a csv format and can be refactored to work with any election. As of now it is designed to be run for voter data in regards to counties. This can be changed if more data is provided. We can add if statements within the iterations of each row to help with other classifications of data. Such as districts, zip codes, age of voters, and etc. 

- Example: 
'''
	districts = []
	district_votes = {}

	if district_name not in districts:
		districts.append(district_name)
		
		district_votes[district_name] = 0

'''

- Example 2:
	Also, changing the labels to match up with the data provided and/or being analyzed. Whether it's a state election, county election, etc. This helps make it easier to decipher the results of the analysis. 
	'''
	state_results = (f'{state}: {state_percentage:.1f}% ({state_votes[state]:,})\n')
	'''


