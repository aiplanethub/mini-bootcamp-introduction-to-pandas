# Sorting

* Assume you are a teacher and you have scores of your students in the dataset ‘exam_scores’ (say). You want to get the information about all the students whose performance is very bad in ‘math’.

* What about going through all the records in the dataset and finding out manually the students whose score in math is very bad?

* You can think of doing this manual task if you have 10 or 20 records. But here you have 1000 records. You need to figure out some easy way to do this. This is where the importance of sorting comes in.

* The data present in the DataFrame ‘exam_scores’ is in the default index order not in a value order.

* Pandas provides a method called sort_values() which returns the sorted result in value order.

* Let's say we want to get the student's information which are in increasing order of math scores.






![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_666996ea4ddf493da6f0bddd553b20bb.png)



* By default the sorting happens in an ascending order:





![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_3d293b7d841444e78935111b8d7c7077.png)





* We can get the sorted result in descending (decreasing) order by passing the parameter ‘ascending’ as False in the sort_values() method:





![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_93cd7f53660d4876bcbb74b1ef02b43a.png)


* We can also sort a series using the sort_values() method:

![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_be108f0c1497413cbca177285e38814f.png)