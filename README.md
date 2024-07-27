1. Data wrangling in Python!
2. Data exploration : from google.colab import drive 
                   drive.mount('/content/drive’)
3. dataset_1=pd.read_csv('/content/drive/MyDrive/dataset_1.csv') # load first dataset
4. Dealing with missing values : drop unnamed column , because they have similar value of serial numbers .
5. Combine_data=pd.merge(dataset_1,dataset_2,on='instant',how='inner') # merge two datasets
5. check for null values
6. Filtering data: dataset_2.drop('Unnamed: 0',axis=1) # drop unnamed column
7. At last we concat the combine_data with dataset_3 by axis=1
8. concat_data=pd.concat([combine_data,dataset_3],axis=1) # concat two datasets
9. Here we work on missing values and drop unnecessary column and find correlation matrix 
10. concat_data.describe() # describe of concat_data
11. Here is describe method is very import to find central tendency.
12. My last task is to performing the pair plot :
13. sns.pairplot(concat_data) # pairplot
