# Challenge_03
Python Election Polling Analysis

# election.analysis

## Overview of Election Audit
Colorado Board of Elections has assigned our team with the task of performing an audit of the congressional election. The Board has asked for the following deliverables:

1. Tabulate total votes cast.
2. Compile complete list of all candidates on the ballot who received votes.
3. Calculate total votes for each candidate.
4. Calculate the percentage of votes received.
5. Determine the winning candidate.
6. Determine voter turnout by county.

## Resources
- Data source provided by the CO Elections Board (election_results.csv)
- Analysis completed with Python 3.8.8 and Visual Studio

## Summary

### Election Audit Results

#### Total Votes Cast: 369,711
    ----------------------------------
    - Charles Casper Stockham: 23.05% and 85,213 votes.
    - Diana DeGette: 73.81% and 272,892 votes.
    - Raymon Anthony Doane: 3.14% and 11,606 votes.
    ----------------------------------
    
    - Winner: Diana DeGette
    - Winning vote count: 272,892
    - Winning percentage: 73.81%
    ----------------------------------

#### County Level Summary    
    Largest county turnout: Denver
    ----------------------------------
    
    - Jefferson: 10.5% (38,855)
    - Denver: 82.8% (306,055)
    - Arapahoe: 6.7% (24,801)
    ----------------------------------
link to election results file: 
    
 
## Election-Audit Summary
 
Our team proposes that the script written for this election audit is modified and used more broadly as a tool for future elections. 
We propose the following changes:
  1. Collect total registered voters by county to calculate the true voter turnout 
```python
county_vote_percentage = float(county_vote)/ float(total_votes) * 100

# change 'total_votes' to 'registered_voters' 
```
  2. Use a master list to cross reference county names from the election_results.csv file to confirm there are no errors in the data.
  3. Adapt code for use with city elections.

link to Python code: <PyPoll_Challenge.py>
