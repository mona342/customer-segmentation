# customer-segmentation
Customer Segmentation

The Python code is conducting exploratory data analysis (EDA) on the Mall Customers dataset to perform customer segmentation. Here's a brief explanation of the purpose of each section of the code:

1. Importing Required Libraries:
The necessary libraries, such as NumPy for numerical computations, Pandas for data manipulation and analysis, and Matplotlib and Seaborn for data visualization, are imported.

2. Loading the Dataset:
The Mall Customers dataset is read from a CSV file using Pandas' read_csv() function.

3. Removing Unnecessary Columns:
The "CustomerID" column is dropped from the dataset using the drop() function with the axis parameter set to 1 (columns) and inplace parameter set to True to modify the original dataframe.

4. Visualizing the Data Distribution:
To understand the data distribution, various visualizations are created:

   - A violin plot is generated for the "Age" column using Seaborn's violinplot() function to depict the frequency distribution of different ages.
   
   - Two boxplots are created, one for the "Spending Score (1-100)" and the other for the "Annual Income (k$)" columns, using Seaborn's boxplot() function to visualize the distribution of these variables.
   
   - A barplot is generated to display the count of customers for each gender.
   
   - Age groups are created, and a barplot is generated to show the count of customers in each age group.
   
   - Spending score and annual income groups are created, and barplots are generated to display the count of customers in each group.

5. Clustering the Data:
The K-means clustering algorithm is applied to the dataset using the KMeans() function from the sklearn library.

   - The optimal number of clusters is determined by calculating the within-cluster sum of squares (WCSS) for different values of K (number of clusters) using the elbow method.
   
   - The dataset is labeled based on the clusters obtained, and a 3D scatter plot is created to visualize the relationship between age, annual income, and spending score for each cluster.
