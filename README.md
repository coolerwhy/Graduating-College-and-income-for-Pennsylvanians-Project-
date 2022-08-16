# Graduating-College-and-income-for-Pennsylvanians-Project-
#Interested in exploring the relationship between graduating college and income for Pennsylvanians.  Two datasets can be helpful. The first is a list of median household income by zip code for the entire US (as well as population and mean household income). These data can be found in the file Median Income by Zip Code in US.xlsx. The second file lists the the percent of residents of each zip code in Pennsylvania who are college graduates. The file also contains the city name associated with that zip code. These data can be found in the file PA College Graduation By Zip Code.xlsx.

1) Read in each file into SAS.
2) Merge the two files together by zip code. When doing so, create three output datasets – one called match that contains only those zip codes that were in both files, a second one called noinc that includes zip codes that don’t have income data, and a third one called nograd that includes zip codes that don’t have college graduation data.
3) How many zip codes are in each of the three datasets that you created above? For the noinc and nograd datasets, speculate as to why these values did not match. You might need to look at the zip codes themselves to figure this out. (I found a website called zip-codes.com that helped me answer this question. If you enter the zip code in the “Free Zip Code Finder” section, information on that zip code will appear. If you are not familiar with how US Zip codes work, please come see me and I’m happy to offer some guidance).
4) Using only the match dataset...
a) Calculate the quartiles of the college graduation rate variable.
b) Create a new variable called CollGradGroup which takes on the following values: 4 if the graduation rate for that zip code is greater than the third quartile
3 if the graduation rate for that zip code is between the median & the third
quartile
2 if the graduation rate for that zip code is between the first quartile & the median 1 if the graduation rate for that zip code is lower than the first quartile
. (that’s a missing value) if the graduation rate is not given
Format the CollGradGroup variable to name the groups “high”, “med-high”, “med-low”, and “low”, respectively. Add a label to the variable as well.
c) You are interested in calculating the mean value of the median income variable as well as the mean value of the population variable separately for each CollGradGroup value. (Thus, you want the mean income for high, med-high, med-low, and low as well as the mean population for each of them as well). Create this in three ways:
i) As a SAS dataset, where the variables are meaninc and meanpop.
ii) In a table using PROC TABULATE.
iii) In a scatterplot, where x = meanpop and y = meaninc. Comment on the pattern that you that you see in the graph.
