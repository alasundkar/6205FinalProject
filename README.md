# EPL RANKING-SYSTEM
6205FinalProject

@authors

NUID: 001316769 :    [deepak_lokwani](https://www.linkedin.com/in/deepaklokwani1/)    
NUID: 001304532:    [rupesh_alasundkar](https://www.linkedin.com/in/rupeshalasundkar/)
 
  ##test comment
 # How start project:
 
 Clone this repository to your local system: 
 

```bash
   git clone    https://github.com/alasundkar/6205FinalProject.git
```

## BEFORE RUNNING

Build your own project before running as this project doesn't contain a .classpath file


## Start program using java command

 ```bash
 java  Driver.java
``` 

# TESTING AND RUNNING THE PROGRAM
## PART I: LEAGUE POINT TABLE

#Step 1:

Firstly, when the main class (Driver.java) is run, a console output is thrown asking
user to choose the method to rank the teams and create a point table.
A user can input either method A or B.

METHOD A: It computes the point table based on the cumulative probability distribution function of a team winning 

METHOD B: It computes the point table based on the discrete probability of each each goal score combination and then takes the decision

Authors prefer Method B for finer accuracy but it is left to user to make a choice 

INPUT REQUIRED: A or B

OUTPUT EXPECTED: A FINAL POINT TABLE FOR THE LEAGUE

## PART II: Face-off Probability Distribution Function

Here the console asks the user to input two teams, home and away team.

INPUT REQUIRED: Home Team

INPUT REQUIRED: Away Team

User is advised to type the names correctly as the input data are names and are case-sensitive

OUTPUT EXPECTED: Output predicts the face-off result of the match if played between the two teams chosen by the user. 

The output shows the following results in order:

a. Goals prediction of home team

b. Goals prediction of away team

c. Probability distribution function over different combinations of the final
score

d. Final score with the maximum probability(discrete)

e. Cumulative probability of a team winning, losing or match drawing based
on the above discrete probability functions
 
Note: The percentage probability almost always adds up to 100% giving us a
hint of the correctness of the calculations

# Design Factors:

Project: Predictive Ranking System of English Premiere League

Factors Considered: 

Location - Home or Away 

Attack Strength - goal scoring ability 

Defense Strength - goal conceding weakness



## Driver Class:
This is my main class. It initiates all the pre-requisite functions that are
required to tabulate the final point table. The driver constructor initially
runs and makes assigns the combination id to each of the match that is played
or is supposed to played.
 
This class contains the algorithm design for predicting the ranking of all
the clubs playing in the EPL based on the previous records of the current
season.
 
This class contains two such methods, the details of which are explained in
detail in the project report or the readme file


## MakePairs Class:
this class makes the pairs of team to face a match and each match to be played 
or already played is given a combination ID and is stored in a HashMap
All the pairs are grouped of tw, played or not played
 

Factors Considered:

Location - Home or Away

Attack Strength - goal scoring ability

Defense Strength - goal conceding weakness


## RankingSystem Class: 
this class is primarily my CSV file reader of sorts. It reads all the
required data values that would be required further in the driver class for
the calculation of the PDF of a match results



## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
