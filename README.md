# FreeCodeCamp: 5 Python Data Projects for Data Analysis with Python Certification

### These are the 5 Python projects formulated by [FreeCodeCamp](https://www.freecodecamp.org/learn) for their Data Analysis with Python course. FreeCodeCamp provides free video tutorials, articles, and projects for programming.

## 1: Mean-Variance-Standard Deviation Calculator
<img src="FreeCodeCampPythonDataAnalysis/Standard_Deviation_Calculator.PNG" alt="standard_deviation" width="640">
The goal of this project was to convert a 9-character Python string into a 3x6 Numpy array of mathematical calculations. I took a unique approach, first converting the 1x9 python list into a 3x3 Numpy array.

<img src="FreeCodeCampPythonDataAnalysis/Standard_Deviation_Calculator_Images/Calculator_1.PNG" alt="Calculator1" width="640">

Next, I found the locations of all the values for performing the calculations. This was pretty straightforward. I created a variable for each value in the final array, specifying the rows and columns for each calculation.

<img src="FreeCodeCampPythonDataAnalysis/Standard_Deviation_Calculator_Images/Calculator_2.PNG" alt="Calculator2" width="640">

Finally, I just needed to format the output. This included the names of the calculations I performed and the variables I had set earlier to display the resulting calculations in the 3x6 array. 

<img src="FreeCodeCampPythonDataAnalysis/Standard_Deviation_Calculator_Images/Calculator_3.PNG" alt="Calculator3" width="640">

[Mean-Variance-Standard Deviation Calculator Code](https://github.com/WillPepperr/Free_Code_Camp_Python_Data_Analysis_Projects/blob/main/FreeCodeCampPythonDataAnalysis/ProjectCode/Mean_Variance_STD_Code)

## 2: Demographic Data Analyzer
<img src="FreeCodeCampPythonDataAnalysis/Demographic_Data_Analyzer.PNG" alt="demographic_data" width="640">
My next project involved loading a CSV into Python using the Pandas library to perform a variety of calculations on a demographic dataset. 

<img src="FreeCodeCampPythonDataAnalysis/Demographic_Data_Analyzer/Demographic_1.PNG" alt="Demographic1" width="640">

Examples of calculations this project required were: average male age, percentage of people with advanced education, and percentage earning a salary threshold of $50,000 annually with and without education. 

<img src="FreeCodeCampPythonDataAnalysis/Demographic_Data_Analyzer/Demographic_2.PNG" alt="Demographic2" width="640">

My approach to this problem was to assign a variable to perform the calculation and set that variable equal to the variable given by the problem's author. This helped me read and understand the calculations I was performing, and keep a clean and consistent aesthetic to the code.

<img src="FreeCodeCampPythonDataAnalysis/Demographic_Data_Analyzer/Demographic_3.PNG" alt="Demographic3" width="640">

[Demographic Data Analyzer Code](https://github.com/WillPepperr/Free_Code_Camp_Python_Data_Analysis_Projects/blob/main/FreeCodeCampPythonDataAnalysis/ProjectCode/Mean_Variance_STD_Code)

## 3: Medical Data Visualizer

This project introduced Data Visualization using Matplotlib and Seaborn libraries, visualizing biometric results to explore the relationship of multiple variables including  cardiac disease, blood markers, and lifestyle choices.


The first step was to import the data and add an 'overweight' metric using a basic BMI calculation based on individual weight and height. This was followed by normalizing the cholesterol and glucose levels to normal or high.

<img src="FreeCodeCampPythonDataAnalysis/MedicalDataVIsualizer/Medical_Data_Visualizer1.PNG" alt="Medical1" width="640">

Now that the data is formatted correctly, I need to draw the first graph, a cat plot. I first added the metrics needed to be plotted, then I used the .groupby() function to compare those who perform cardio exercise regularly and those who do not. Then the Seaborn plot is called to display the graph.

<img src="FreeCodeCampPythonDataAnalysis/MedicalDataVIsualizer/Medical_Data_Visualizer1b.PNG" alt="Medical1b" width="640">

<img src="FreeCodeCampPythonDataAnalysis/MedicalDataVIsualizer/catplot.png" alt="catplott" width="640">

For the heat map, the author wants the data cleaned first. to perform this the bottom 2.5% and top 97.5% of height values will be removed for an accurate result.

<img src="FreeCodeCampPythonDataAnalysis/MedicalDataVIsualizer/Medical_Data_Visualizer2.PNG" alt="Medical2" width="640">

Before the heat map can be displayed, a couple of values need to be assigned. This includes the correlation method and a mask. Afterwards the Seaborn heatmap() function can be called, displaying the heat map.

<img src="FreeCodeCampPythonDataAnalysis/MedicalDataVIsualizer/Medical_Data_Visualizer3.PNG" alt="Medical3" width="640">
<img src="FreeCodeCampPythonDataAnalysis/MedicalDataVIsualizer/heatmap.png" alt="heatmap" width="640">

[Medical Data Visualizer Code](https://github.com/WillPepperr/Free_Code_Camp_Python_Data_Analysis_Projects/blob/main/FreeCodeCampPythonDataAnalysis/ProjectCode/Medical_Data_Visualizer_Code)

## 4: Page View Time Series Visualizer
For this project, I am given data on page views in a CSV for the FreeCodeCamp website including daily visit numbers. First I import the CSV and clean the data removing the same 2.5% and 97.5% quantile from the dataset. 

<img src="FreeCodeCampPythonDataAnalysis/Time_Series_Images/Time_Series_1.PNG" alt="TimeSeries1" width="640">

Next, I draw a line plot. This is very straightforward using Matplotlib. I simply call the function import the dataframe, and set the correct labeling.

<img src="FreeCodeCampPythonDataAnalysis/Time_Series_Images/Time_Series_2.PNG" alt="TimeSeries2" width="640">

<img src="FreeCodeCampPythonDataAnalysis/TimeSeriesImages/line_plot.png" alt="lineplot" width="640">

The second plot required is a bar plot. This will group each year and display a bar for the average daily views each month. I do this with the 'groupby()' function, and then I call the 'bar.plot()' function and list the months as the legend.

<img src="FreeCodeCampPythonDataAnalysis/Time_Series_Images/Time_Series_3.PNG" alt="TimeSeries3" width="640">

<img src="FreeCodeCampPythonDataAnalysis/TimeSeriesImages/bar_plot.png" alt="barplot" width="640">

Finally, there needs to be a box plot containing 2 graphs. One that shows the trend by drawing a box and whiskers for each year, and one that has a box and whiskers for the 12 months. I do this by setting the month number to the correlated name and drawing the boxplots on 2 different axes. The year plot is 'axis[0]' and the monthly is 'axis[1]'.

<img src="FreeCodeCampPythonDataAnalysis/Time_Series_Images/Time_Series_4.PNG" alt="TimeSeries4" width="640">

<img src="FreeCodeCampPythonDataAnalysis/TimeSeriesImages/box_plot.png" alt="boxplot" width="640">

[Page View Time Series Visualizer Code](https://github.com/WillPepperr/Free_Code_Camp_Python_Data_Analysis_Projects/blob/main/FreeCodeCampPythonDataAnalysis/ProjectCode/Time_Series_Visualizer_Code)

## 5: Time View Sea Level Predictor
The last project of the certification includes a file containing sea level measurements each year. A scatterplot with 2 trendline calculations needs to be created. After importing the CSV, I set the X and Y values to year and the sea level measurement. Then I can use the 'linregress()' function to calculate the trendline using data from all the dates provided.

<img src="FreeCodeCampPythonDataAnalysis/Sea_Level_Predictor/Sea_Level_Predictor_1.PNG" alt="Sea1" width="640">

After this, another 'linregress()' line is created, but this time just using data after 2000. When visualized, it shows a much sharper increase. Finally all that's left is labeling the axes and setting the title.

<img src="FreeCodeCampPythonDataAnalysis/Sea_Level_Predictor/Sea_Level_Predictor_2.PNG" alt="Sea2" width="640">

![sea_level_plot](FreeCodeCampPythonDataAnalysis/sea_level_plot.png)

[Time View Swa Level Predictor Code](https://github.com/WillPepperr/Free_Code_Camp_Python_Data_Analysis_Projects/blob/main/FreeCodeCampPythonDataAnalysis/ProjectCode/Time_Series_Visualizer_Code)

## Final Thoughts
I really enjoyed working on these Python data projects! I thought they were challenging enough to figure out, but the libraries make the actual written code concise and easy to understand. I would like to thank FreeCodeCamp for the structured lessons and project materials. It was a great introduction to utilizing common Python libraries for data analysis, and I look forward to learning more about code and doing more projects with Python!
