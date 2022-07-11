# Selecting

## Attribute (Dot) Based Selection

* We used the shape attribute to know the shape of the DataFrame. Do you recall this? If you don't remember, follow the code below.









![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_36ff3156ecea49e69344738d276dc835.png)









* Similarly, you can use a particular column name as an attribute to select a column.

## Dictionary (Bracket) Based Selection

* Do you recall getting a value from a dictionary using a key? If you don't remember, follow the code below.









![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_a15ca5aae63e4136a75e459b947b484a.png)







* Similarly, you can use a column name to select a column from a DataFrame: **` df['column_name']`**

## Selecting Multiple Columns

* While selecting multiple columns, we use double square brackets [[]].









![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_3722b9eae6614e6c9e6adaff467205af.png)









## Conditional Selection

* Suppose you are interested in getting data of 'Jose' from the given DataFrame.





![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_3bc41f8f29704635bc3fd005fb5e99bb.png)




* We can make a condition using any conditional operators discussed in the 'Introduction to Python' course. Let's say we want the record where the 'Name' is 'Jose'. We can use a condition here using the **`==`** conditional operator.

* This will return a series of True/False values:




![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_3a3819cd4a314f979020454c7f08dcf4.png)




* Get all the columns of the row that satisfies the condition. Here the condition is to get the rows where the Name is 'Jose'.



![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_3d2d8eb748714e0aa70f2c9a8b396967.png)