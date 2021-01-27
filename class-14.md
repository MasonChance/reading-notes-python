# Matplotlib: using pyplot

here we will look at a high level overview of  matplotlib basics, for further detail and advanced topics see the [matplotlib tutorials](https://matplotlib.org/tutorials/index.html) and their [Documentation](https://matplotlib.org/contents.html#)

For ease of reference the matplotlib will be referred to as 'mtplt' throughout this document. This is not to be confused with the conventional alias `plt` used in actual code. 

mtplt uses figures to graph data the basic way to create a figure after importing mtplt is with `subplots()` method. 
>>
  import matplotlib.pyplot as plt

  fig, ax = plt.subplots() # creates a figure with a single axis. 
  ax.plt([list_of_x-axis_values], [corresponding_list_of_y-axis_values])

>>

It is important to note that when creating the `figure` with the `subplots()` method the 'single axis' the comment reffers to is the axis on which the figures appear. the actual plot called with `ax.plot` can have as many axes as necessary for the data you wish to visualize. 

mtplt does have some built-in short-cuts, in that one could create a plot without explicitly createing the figure and figure axes. 
` plt.plot([list_of_x-axis], [list_y-axis])` but in the event that you want to display the figures on the same line or cell etc, it is useful to know the longhand way of doing it. 


there are a great many things we could go over but I want to point you to ![the anatomy of a plot](https://matplotlib.org/_images/anatomy.png)

by understanding this it will be a lot easier to understand the methods and the arguments they require when working with matplotlib.

below are a few key things you will want to familiarize yourself with in the tutorial and documentation. 

- the types of Input plotting functions accept: 
  - numpy.array or numpy masked_array. matrixes and dataframe objects may not work as intended, converting before passing is best. 
- wheather you need to explicitly create your plots and figures or rely on pyplot to infer the necessary layout, labels, and other details
- there is a different process for plotting if the plots need to be embedded in a GUI, see [Embeding matplotlib in graphic user interface](https://matplotlib.org/gallery/index.html#user-interfaces) for more details regarding this. 

- if you will need to use the same plot structure for multiple datasets, it is recomended to use a function, a reccomended function signature can be found in the usage guide tutorial.







#### [Return to Main index of Notes](./README.md)