# My Code: cleanCode.Scala
My cleaning code for my half of cleaning the NFL Datasets for my PBDAA Final Project

## How to Run: This code can be ran in Spark using the command below.
spark-shell --deploy-mode client -i  cleanCode.scala

## Code Purpose:
The code will clean allcombineData.csv (my combined dataset) by getting rid of all columns except Player,Pos,40yd and create a new column called round which gets the round value for each player in the data 
by parsing through the original Drafted(tm/rnd/year) column. It will also only keep Players that have the 
Position: QB, WR, TE, RB and also Players with a 40yd dash time. The code will write this to a new csv file 
which will be called cleanedCombineData.csv.  This new file is the finalized and is now a perfectly cleaned dataset 
that can then be used for further analytic purposes. 
