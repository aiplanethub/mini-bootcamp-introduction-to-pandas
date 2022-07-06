# Indexing


## What is Indexing in Pandas?

* Indexing in Pandas means selecting particular rows and columns from a DataFrame.
* Indexing in Pandas is same as we did for a Python List and a NumPy array.
* There are two different methods of indexing in Pandas:
  * **loc - label based selection**
  * **iloc - index based selection**



## Index Based Selection

* Index based selection is to select data based on its numerical position in DataFrame.
* **iloc** is used for selecting data based on numerical position.
* The syntax for using **iloc** operator is **`df.iloc[ ]`**, where df is a DataFrame name. You can pass the numerical positions of rows and columns to select in the square bracket.
* Do you remember the indexing in a NumPy array? If not, don’t worry, you will soon see its implementation on a dataset.
* Import Pandas Library and load ‘exam_scores.csv’ file







![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_a3d990f7c8c94259857691ac671a6c15.png)




### Selecting data using iloc:






![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_fe485c44a4b14d00aac41d1c33a6b5e5.png)










![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_5200cda812bb4dd884a98726cb1acb67.png)



* You can also pass **list of indexes**



![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_c6ec5a15776f47d6ad092b9580fd62c3.png)




* You can also pass **negative indexes**




![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_38ff8f42a4bb4b9b8a025fdc51858115.png)




## Label Based Selection

* Label based selection selects data based on the column or row names/index. This becomes important while selecting data from a DataFrame.
* Label based selection is done with loc.
* Do you remember the python default indexing of the DataFrame and the indexes/names that you changed in the previous topics?
* loc and iloc are conceptually similar. The difference is that iloc considers the default indexing while loc ignores the default indexing.
* **loc** is used for selecting data based on the data index value/name, not the numerical positions.
* The syntax for loc is similar to iloc: **`df.loc[ ]`**, df is the DataFrame name.
* We will learn about its implementation on a dataset soon.

### Selecting data using loc:

![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_cf0e74eeae2d48f28653564538e81018.png)