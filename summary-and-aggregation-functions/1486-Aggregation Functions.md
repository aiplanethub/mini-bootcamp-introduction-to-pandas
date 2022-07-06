# Aggregation Functions



* We saw the use of **describe()** method on a DataFrame or a series which returned some information (i.e. the summary) about the data.
* We can also use the individual methods like **mean(), median(), unique()** to get this information on a DataFrame or a series.
* Examples are shown below:






![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_d88804e031c540099b147c3c0fa13aeb.png)






* To see all the unique values and the number of times they are occurring in the dataset, we have a method called value_counts():


![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_c40daa0935f646fda57887659160ff5c.png)

* 'female' is occurring 502 times in gender column which we saw in the table returned using describe() method as well.