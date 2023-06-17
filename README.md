# kevin-joshi-assigment

The code starts by importing the required libraries, including pandas and matplotlib.

It reads an Excel file using the pd.read_excel() function and assigns the data to a DataFrame called df.

The code then plots time series data for columns 'r1' to 'r12' and the 'temp' column using a for loop and the plt.plot() function from matplotlib. Each 'r' column represents rainfall data for a specific region.

The plot is customized with labels for the x-axis, y-axis, and legend. Finally, the plot is displayed using plt.show().

Next, the code imports the KMeans class from the sklearn.cluster module to perform clustering on the 'r1' to 'r12' columns of the DataFrame.

It selects the rainfall columns ('r1' to 'r12') and applies the K-means clustering algorithm with n_clusters=5 to cluster the data.

The resulting cluster labels are assigned to a new column 'cluster' in the DataFrame.

The code prints the count of data points in each cluster using df['cluster'].value_counts().

Finally, the code displays the updated DataFrame with the 'cluster' column.
