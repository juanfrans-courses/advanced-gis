#Answers to the Spatial Statistics Assignments (part 1 and 2)

###Spatial Statistics Assignment_01
1. Using the Nearest Neighbor form of pattern analysis answer the following questions: Does the 311 noise complaints overall exhibit a dispersed, clustered or random pattern? How do you know? At what confidence level can you say this? Does this make sense by looking at the data? (Hint, think about the in class exercise to determine your area.) Provide your test results.
    * Here, to measure whether the 311 noise complaints exhibit an overall dispersion, clustered or random pattern, we use the ‘Average Nearest Neighbor’ tool which measures to see if the physical locations are closer together than they would be expected with a random distribution. For the area, within the tool, use the cumulative square footage of the five boroughs. For the sub-questions, analyze and infer the confidence level from the resulting graph and distribution chart. 

2. Do any of the subcategories represented in the “descr” field exhibit clustering? If so, which ones? Provide your test results for each one of the categories.
      * Use the same tool for this question with specific categories from within the ‘descr’ field, one at a time, and read the results to understand if the categories exhibit clustering within the field. 

3. We want to know whether addresses where there are repeat calls to 311 also cluster in the data set. In other words do addresses that call 311 often cluster? (Hint, this is where you may want to use the collect events tool.) If they do, is there a distance in which clustering is more exhibited? Why do you think you see this pattern? Please create a chart showing clustering results at six different distances. Please be strategic in selecting distances used; why did you choose them? Is there anything expected or unexpected about the results you generated?
      * Using the ‘collect events’ tool for the first part of the question, differentiate those points which make 311 calls often (calls>1). There are various ways of proceeding with this analysis. Using the ‘Multidistance Clustering’ we can understand the variation of distance at which clustering is occurring, by trying a couple of different distance bands and increments. This gives us a fair idea about the distance where the clustering peaks. Using this and keeping the Manhattan block size in mind (always refer to the city fabric you are working with) we choose 6 distances and perform the ‘Getis Ord General G’ tool. This tool helps to see if there are areas where similar values are closer together than would be expected with a random distribution. We can also use the ‘Getis Ord General G’ tool directly after the collect events tool by choosing 6 distances as discussed above.

4. What is the null hypothesis for the tests you were performing above?

A4. The null hypothesis for the tests is: The 311 call events are random – 

neither dispersed nor clustered.

Spatial Statistics Assignment_02:

1. Find the community district with the most noise complaints (hint: you will have to 

join your data to the community district file). Does this community district also 

represent an area that might be considered a noise hotspot - an area where the 

concentration of high noise level is statistically significant? (Hint: you will have to 

perform a statistical analysis). Create one map showing these results.

A1. First join the noise complaint data to the community district file, and using 

the ‘Hot Spot Analysis’ tool perform the analysis. The results with depict the 

confidence level for each hot spot and will also give a Gi-Z score in the 

attribute table to analyze the concentration statistically.

2. Take the two community districts with the greatest number of noise complaints 

and perform a more neighborhood-level analysis about what might be causing 

the high number of complaints in these areas. One suggestion is to join the 311 

data to the New York City Blocks or Parcels files and search for hotspots at the 

community district level. Make sure you pull out just the neighborhood, otherwise 

if you are working with the file for the whole city the analysis will never finish. Are 

there locations within the community districts that represent neighborhood-level 

hotspots? What are those areas? How significant is the cluster (please, respond 

this question with the statistical data you generated)? Do the hotspots appear to 

correspond to a specific concentration of a certain type of land-use (it is not 

necessary to perform a statistical analysis on the land use data, a visual analysis 

and interpretation is all that is needed)? Create one map for each community 

district showing both the noise hotspots and the land use data.

A2. Taking the two community districts with the greatest number of noise 

complaints, join the 311 data to the NYC blocks or parcels file. Again, perform 

the hot spot analysis - at the community district level, this time. Through the 

analysis results, locate the neighborhoods that depict significant clustering 

(again, spatially and statistically). By using the PLUTO land-use data for 

these neighborhoods, inference visually any relationship between 

concentration of a certain type of land-use with the hotspots. 

3. What is the difference between these types of analysis and the ones you used 

last week? What does each type of analysis tell you about the data?

A3.The spatial analysis last week, was global statistics analysis where the 

entire data is analyzed to depict clustering, randomization or dispersion for 

the entire region. Whereas this week, the analysis was a local statistics 

analysis, that combines the spatial location with the attribute values to 

perform pattern analysis and pinpoints the locations of clustering patterns.

4. Provide an appendix that describes what you have done: what parameters did 

you specify for each one of your analysis? Please write down your results (show 

the score results). For example, if you used distance bands you should explain 

why you chose the distances that you did. Remember, like last week, you might 

need to perform the same analysis at different distances to find the optimal level 

of clustering.

**Due before the end of Monday, October 26th**
 
This is the second of a 2 part section assignment which will allow us to explore the 311 data about noise complaints in New York City. Using a dataset and a geography we are more familiar with will help us understand some of the logic behind basic spatial statistics.
 
###DATASETS
The datasets that you will use in this assignment are the following:
* Noise complaint file for September 2015 (the same one that you used for your previous assignment)
* New York City Borough’s File. Located at: X:/New_York_City/Boundaries/Borough_Boundaries/nybb_15b/nybb.shp
* New York City Community Distric File. Located at X:/New_York_City/Boundaries/Community_Districts/nycd_15b/nycd.shp
* New York City PLUTO File. Located at X:/New_York_City/Buildings_Lots/Lots/PLUTO/2015_15v1/
* New York City Census Blocks File. Located at X:/New_York_City/Census/Census_Blocks_Tracts_2015/Census_Blocks/nycb2010_15b/
* Any other files you consider necessary for your final maps.
 
###QUESTIONS
In this assignment you will identify noise hotspots and coldspots in New York City (locations where high or low levels of noise appear to be statistically significant). In order to better understand the relationships between the noise complaints and specific areas of the city you will perform a series of exercises and tests:
 1. Find the community district with the most noise complaints (hint: you will have to join your data to the community district file). Does this community district also represent an area that might be considered a noise hotspot - an area where the concentration of high noise level is statistically significant? (Hint: you will have to perform a statistical analysis). Create one map showing these results.
 2. Take the two community districts with the greatest number of noise complaints and perform a more neighborhood-level analysis about what might be causing the high number of complaints in these areas. One suggestion is to join the 311 data to the New York City Blocks or Parcels files and search for hotspots at the community district level. Make sure you pull out just the neighborhood, otherwise if you are working with the file for the whole city the analysis will never finish. Are there locations within the community districts that represent neighborhood-level hotspots? What are those areas? How significant is the cluster (please, respond this question with the statistical data you generated)? Do the hotspots appear to correspond to a specific concentration of a certain type of land-use (it is not necessary to perform a statistical analysis on the land use data, a visual analysis and interpretation is all that is needed)? Create one map for each community district showing both the noise hotspots and the land use data.
 3. What is the difference between these types of analysis and the ones you used last week? What does each type of analysis tell you about the data?
 4. Provide an appendix that describes what you have done: what parameters did you specify for each one of your analysis? Please write down your results (show the score results). For example, if you used distance bands you should explain why you chose the distances that you did. Remember, like last week, you might need to perform the same analysis at different distances to find the optimal level of clustering.

###DELIVERABLES
One **PRINTED** board (24x36 or something similar) with the three maps and brief texts describing each one of them, and one PDF appendix with your calculations. Again, think about your layout, titles, fonts, legend, scales, north arrows, labels and use of color. Practice your layout and design skills and make one board that is both clear and interesting. A PDF copy of your printed board and the appendix should be uploaded to Courseworks before the end of Monday, October 26th.

###NOTE
***Printing at GSAPP takes a while, so early on figure out how to submit files to the print shop and what the turnaround time is. Don't leave it for last minute.***
