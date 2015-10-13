#Spatial Statistics Assignment
###Understanding New York City 311 Noise Data (Part 1)


*Due before the end of Sunday, March 8th*

This is the first of a 2 part section assignment which will allow us to explore the 311 data about noise complaints in New York City. Using a dataset and a geography we are more familiar with will help us understand some of the logic behind basic spatial statistics.

#DATASETS
The datasets that you will use in this assignment are the following:
1. Noise Complaint File for October 2010. Located at: GIS_Classes/A6232_Adv_GIS_SP2015/02_Tutorials/04_Spatial_Statistics_1/Assignment_Data/311_oct2010noisecomplaints.shp
(The “descr” is the category description of the complaints.)
2. New York City Borough’s File. Located at:
GIS_Classes/A6232_Adv_GIS_SP2015/02_Tutorials/04_Spatial_Statistics_1/Assignment_Data/bboundary.shp
 
#NOTE
If you want to see if there are addresses with repeat complaints you can use the “collect events” tool. This tool will collect all the points that happen at the same location into one single point and give it a value field indicating how many points were collected at that same location. It’s a great tool for when you are working with point data.

#QUESTIONS
1. Using the Nearest Neighbor form of pattern analysis answer the following questions: Does the 311 noise complaints overall exhibit a dispersed, clustered or random pattern? How do you know? At what confidence level can you say this? Does this make sense by looking at the data? (Hint, think about the in class exercise to determine your area.) Provide your test results.
2. Do any of the subcategories represented in the “descr” field exhibit clustering? If so, which ones? Provide your test results for each one of the categories.
3. We want to know whether addresses where there are repeat calls to 311 also cluster in the data set. In other words do addresses that call 311 often cluster?  (Hint, this is where you may want to use the collect events tool.) If they do, is there a distance in which clustering is more exhibited? Why do you think you see this pattern? Please create a chart showing clustering results at six different distances. Please be strategic in selecting distances used; why did you choose them? Is there anything expected or unexpected about the results you generated?
4. What is the null hypothesis for the tests you were performing above?
 
#DELIVERABLES
No map is required for this assignment. Instead, you should provide a PDF document answering the questions and displaying your charts and data. The document should be uploaded to Courseworks before the end of Sunday, March 8th.
