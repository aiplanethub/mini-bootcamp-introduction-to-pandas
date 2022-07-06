# Missing Data

## What is a Missing Value?

* If in any row or column in a DataFrame, a value is not available, it is said to be a missing value.
* So, defining missing data: **Missing data (or missing values) is defined as the data values that are not stored in a column or row.**
* Consider this small dataset which has some missing values in it (shown in the red box).






![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_795aef8e95a64899a44828316050f089.png)






* Well this is a small dataset so we can easily observe the missing values here. But real-world data is very large in size and you cannot easily see the missing values in the DataFrame.
* Pandas provides **isnull(), isna()** functions to detect missing values. Both of them do the same thing.

* **df.isna()** or **df.isnull()** returns the DataFrame with Boolean values indicating whether a value is missing (True) or not (False).






![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_08e1d3dd0780454c89f91c907725e273.png)





* We can get column wise count of all the missing values using the aggregation function **sum()**:


![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_9b65636cf67744b5bf1d58e5135e2b67.png)



* Both the columns 'Names' and 'Marks%' have one missing value each. 'Regd. No' has no missing values so the value is 0.

* Pandas also provides **fillna()** method to fill the missing values. fillna() provides many different strategies to fill missing values.

* Let's say we want to fill the missing values in 'Names' column with 'unknown'.



![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_832c39b0215b4e199dbbbcc202a25713.png)



* But the changes are not made in-place. The DataFrame still contains missing values in the 'Names' column.











![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_5cdb4107313a4908a8682d1071dae4cc.png)









* We can pass 'inplace' parameter as True in fillna() method. It will make the changes in the original DataFrame.





![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_216e4139f0734660bc5d8f32ed87763c.png)





* There is still a missing value in 'Marks%' column. Let's say we want to fill the missing value in this column with the mean of the marks scored by other people.



![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_7d94aa2562c24b918522e6607bfef948.png)


* Now, our DataFrame has no missing values.

The quiz on the next page uses the following dataset: [Titanic Dataset](https://github.com/dphi-official/Datasets/blob/master/titanic_data.csv)