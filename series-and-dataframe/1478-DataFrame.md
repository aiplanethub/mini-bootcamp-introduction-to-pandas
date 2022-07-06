# DataFrame

## Learning Objectives

* What is DataFrame?
* Create a DataFrame

## What is a DataFrame?

* Two dimensional table
* Made up of a collection of Series
* Structured with labeled axes (rows and columns)

A data frame looks like a table as shown in the image here:










![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_ebaddd603f8d4917abf0f77bbc358eeb.png)










## Create a DataFrame

* You can create a DataFrame using a Python list or a NumPy array:








![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_7365e26062974270be514dc0d7a0963f.png)







* Exercise: Try creating a DataFrame using a NumPy array.
* **Don’t like python default index starting from ‘0’?** Well, you can give your own column and row indexes:






![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_cbcd08ba73904b2d882dea2d06283a31.png)





* **You can create a DataFrame using dictionary:**







![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_1064cc0cabc74eb985e5d95c7be8c6a0.png)







## A Column is a Series

* A DataFrame is a collection of series.
* A series is a column in a table or a DataFrame.

![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_c26c3dfa04f1419d83d73bbb22a8a446.png)

* There are 3 series in the given DataFrame - ‘Regd. No’, ‘Names’ and ‘Marks%’.