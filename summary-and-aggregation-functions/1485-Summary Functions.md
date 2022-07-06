# Summary Functions

## Learned Till Now

So far you have learned reading a data file, some methods to check the overview about data and selecting data from a DataFrame.

  \
This information, that we got about the data, is not enough. A data scientist always wants to understand the behavior of data. For numerical columns we may want to know the mean value or median values of the data, the minimum value in the column and the maximum value in the column, etc. For categorical column we are interested to know things like the number of different categories in a column, the count of each category in a column, the maximum occurring category in a column, etc. Here we will look at some of the techniques that will help you know the above information about your data.

## What is Summary?

* Summary is a term used for short version of a longer work.
* Summary is a brief statement of the main points of something.
* Confusing? Let’s understand through an example.

## Summary Functions

* Pandas has many simple "summary functions" (well, this is not an official name) that help you to restructure your data in a very useful way and displays the useful information about the data.
* Do you recall the **info()** method that we had used in the earlier module? This method has given us 6 to 7 main points about the data like number of observations and their range indices, names of columns with their data types and number of non-null entries in the particular column, etc.
* So **info()** is also a summary function/method.
* Here we will see another summary function - **describe()**.
* Import Pandas Library and load the dataset ‘exam_scores.csv’:





![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_ccbbca4b55fd481e9337994aa9ebc4ee.png)


### describe( )

* describe() method, by default, returns a summary about numerical columns only.






![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_dad18728f9e545589472ffba987f2a66.png)






* Don’t worry if you don’t know what the terms in the red box mean. You will know the meaning of these terms in further content.
* If we want to get a summary about categorical columns separately, then we can use the parameter **'include'**.





![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_3e9ab3df38ff4b5ca7eefb55f3dd70ed.png)



* The returned summary is all about the categorical columns.
* Also, we can get a summary about numerical and categorical columns together using the same parameter **'include'**.







![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_1b49a5a66a3d42b9acebaf377cd3616c.png)




* We can see the above table includes a summary about both numerical and categorical columns. A categorical column cannot have minimum or maximum values or mean and median. So the entries in these fields for categorical columns is **`NaN`**.
* We have seen in a previous module that this dataset has 5 categorical variables (gender, race/ethnicity, parental level of education, lunch and test preparation course) and 3 numerical (i.e., integer) columns (math score, reading score and writing score).







![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_533b3fe1911442b19add60a97f81791a.png)






*   Let's see what information about the data is returned in the above table:

    * **count** - the count of non-null entries in the particular column. For example, gender column has 1000 non-null entries.
    * **unique** - the count of unique values in a column. Only for categorical columns. For example, gender column has 2 unique values - male and female.
    * **top** - this is also for only categorical columns. This tells us which category is occurring maximum number of times. For example in gender column 'female' is occurring maximum number of times.
    * **freq** - this is again for categorical columns only. This tells you the number of occurrences of the top category in that column. For example, 'female' in gender column is occurring 502 times.
    * **mean** - the mean value of the numerical column. For example, the mean math score is 67.128.
    * **std** - this is the standard deviation of the numerical column. This tells you about the variation in the data. Don't worry if you don't know about it.
    * **min** - the minimum value in the numerical column. For example, the minimum math score is 15.0
    * **25%** - the 25th percentile (or 1st quartile) value in the numerical column. For example, the 25th percentile value for math score is 58.0.
    * **50%** - the 50th percentile (or 2nd quartile or the median) value in the numerical column. For example, the median math score is 67.0.
    * **75%** - the 75th percentile (or 3rd quartile) value in the numerical column. For example, the 75th percentile value for math score is 78.0.
    * **max** - the maximum value in the numerical column. For example, the maximum math score is 100.0.
    * **NaN values** means that for a particular column, a particular summary value is not available. For example, gender (a categorical column), does not have mean value or median value as these are the properties of a numerical column only.










* **We can also use describe() method on a particular column/series:**







![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_3f98a4ed20984f239b6b2024605a6464.png)








* If the column name does not contain any space in it, you can use attribute style of selecting a column. For example we used attribute style for selecting 'gender' but not for 'math score' as it contains a space.
* If you use attribute style of selection for ‘math score’, Python will throw an error.



![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_aec4e71c4f0b43ad8510293308d4f9cf.png)