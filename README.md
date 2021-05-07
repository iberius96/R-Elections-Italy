## Purpose of this project

The main goal of this project is to provide a range of visual information regarding the Italian elections for both Chamber and Senate.
During the course of this work we will work with multiple election related features both at the national and regional level.
Additionally, we would like to find out if the employment rates in Italy are a relevant factor in influencing the political direction of the country.

## Notes on translations

For the purpose of this analysis, it has been decided to provide a translation for all Italian terms that we will encounter.
Since many of this terms have a non-univocal translation in English, it has been decided to provide a translation table that goes as follows:

ITALIAN TERM -> TRANSLATION

Scrutinio -> Ballot

Lista (elettorale) -> (Electoral) list

Elettore -> Constituent

Votante -> Voter

Scheda bianca -> Empty vote

Scheda non valida -> Null vote

Camera (dei Deputati) -> Chamber (of Deputies)   

Senato (della Repubblica) -> Senate (of the Republic)

Trasversalismo -> Syncretic (politics)


In the following sections, during the length of the whole project, only the English terms will be used. 
The necessary steps will be taken in order to translate the Italian terms present in the used datasets to their English counterpart.
The name for both political parties and regions have been kept as they appear in the Italian language, even when a possible translation did exist in English (e.g. Sicilia -> Sicily).

## Additional notes

In the context of the used datasets the ballot contains information, for each election year and for both houses (Chamber and Senate), regarding the number of people that CAN vote (constituents) and the number of people that HAVE voted (voters).

The (electoral) list provides the number of votes received by each party during a given election year.

Italy introduced the universal suffrage in 1945 by extending the right to vote to women. 
Since the earliest election year in our dataset is 1948, all votes come from both the male and female population.

All Italian citizen above the age of 18 can vote for the Chamber of Deputies.
Only those who have reached the age of 25 are able to vote for the election of the Senate.

## Information on data sources

Source: Italian Government (https://elezionistorico.interno.gov.it/)

Data: Lists and ballots for national and regional data

Path: ./source/elections/regions, ./source/elections/italy

File(s): lists-Senate-Reg.csv, ballots-Senate-Reg.csv, lists-Chamber-Reg.csv, ballots-Chamber-Reg.csv, ballots-Chamber.csv, lists-Chamber.csv, ballots-Senate.csv, lists-Senate.csv
<br/><br/>
Source: Italian Senate (http://www.senato.it/)

Data: Seats in the Italian Senate

Path: ./source/elections

File(s): senate-seats.csv
<br/><br/>
Source: Wikipedia (https://en.wikipedia.org)

Data: Parties collocation

Path: ./source/elections

File(s): party-collocation.csv
<br/><br/>
Source: ISTAT (https://www4.istat.it/en/)

Data: Employment rates

Path: ./source/labour

File(s): gdp-per-capita.csv

## Note on Shiny applications

The attached .rmd files contains two Shiny applications (line 598-756 and line 1068-1105)
The content of these code blocks is not visible in the .html contained in this folder ("Shiny applications not supported in static R Markdown documents").

Please use RStudio to execute and interact with these two portions of the project.