Data wrangling in Python!
Data exploration : from google.colab import drive 
                   drive.mount('/content/drive’)
dataset_1=pd.read_csv('/content/drive/MyDrive/dataset_1.csv') # load first dataset
Dealing with missing values : drop unnamed column , because they have similar value of serial numbers .
Combine_data=pd.merge(dataset_1,dataset_2,on='instant',how='inner') # merge two datasets
check for null values
Filtering data: dataset_2.drop('Unnamed: 0',axis=1) # drop unnamed column
At last we concat the combine_data with dataset_3 by axis=1
concat_data=pd.concat([combine_data,dataset_3],axis=1) # concat two datasets
Here we work on missing values and drop unnecessary column and find correlation matrix 
concat_data.describe() # describe of concat_data
Here is describe method is very import to find central tendency.
My last task is to performing the pair plot :
sns.pairplot(concat_data) # pairplot
