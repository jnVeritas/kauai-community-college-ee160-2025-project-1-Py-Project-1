# Py-Project-1
A simple data analysis to teach people how to handle data in python.

# Task List:

### 1:
&emsp; Download the file "data11Oct21.csv". This is a .csv file which stands for a 'Comma Separated Variable' file. These files are just text files with a list of values separated by commas. You can open it with any text reader, or even excel to see what it looks like. You'll first few lines are special and they contain some values that need to be handled uniquely.
Start by reading the file into python, and printing the number of lines the file has to the screen.

### 2:
&emsp; Now that you have read the file in, write a function that prints out all of the column headers in alphebetical order.

### 3:
&emsp; Write a new function that takes the column header as an argument, and gives you back a list of all the values in that column.

### 4:
&emsp; Write another two functions that take a column header as an argument. One should give you the maximum and the other the minimum value of the corresponding column.

### 5:
&emsp; The first column in the file is titled "Time(min)". It is the number of minutes elapsed since the creation of the file. There is another column titled "Chamber TC1(C)" that records the temperature of a chamber.
Use pyplot to plot this temperature vs time.

### 6:
&emsp; The temperature is actually recorded by two different devices. There is another column titled "Chamber TC2(C)", which has the second temperature sensor recording.
Use pyplot to plot the second temperature vs time.

### 7:
&emsp; A lot of times, we don't really care what the exact values a detector is giving back. We often care *more* about how big these values are compared to that detector's own maximum. (A value of 2 can be tiny if your detector has a range of 100000, but it can also be huge if your detector has a range of 2.1.) To compare two signals on a more level playing field, it's useful to "normalize" them. To normalize a detector signal, you take each point, and divide it by that detector's maximum value. The result is a signal that always varies between 0 and 1.
Plot the *normalized* temperature vs time.

### 8:
&emsp; When we are talking about how two signals compare to each other, it's also often useful to take time out of the equation and talk about how the two signals relate to each other statistically. One of the more powerful tools for showing this is called a correlation plot. To make a correlation plot for the two temperatures, all we need to do is normalize them both (we did this for one already), and plot the two Y value sets against each other. Two sets that correlate perfectly will form a diagonal line. Any disagreement will show up as a wider cloud of points or some other shape.
Make a correlation plot of the two temperatures. Make sure to use a scatter plot instead of a line. Describe the shape of the plot.

### 9:
&emsp; Sometimes we are more interested in how *different* two detector's values are, rather than what they record on their own...
Plot the *difference* between the two *un-normalized* temperatures vs time.

### 10:
&emsp; Make correlation plots for some of the other columns in the file. (Be careful, you will get an error if you try to normalize something that has a maximum of zero.) Do you see any variables that have a horizontal line as a correlation plot? What does this mean? Do you see any correlation plots that have very strange looking shapes? Without knowing more about this data file, it's hard to say why these weird shapes exist. But any time you see a shape in a correlation plot it means your two detectors have a relationship. Come up with a theory about one of the wierdly shaped plots.
