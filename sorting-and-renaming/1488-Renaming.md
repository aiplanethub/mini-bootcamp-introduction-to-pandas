# Renaming

* Renaming means changing the name.

* Most of the time we get dataset where column names are not satisfactory.

* For example in this dataset, 'math score', 'reading score' and 'writing score' contain spaces in their names due to which we are not able to use attribute (dot) selection style method to select a particular column. 

* And not only this if the column names were 'ms' for math score, 'rs' for reading score and 'ws' for writing score, these are not informative column names. This is the need for renaming columns.

* Pandas provides a function ‘rename()’ to rename column/indexes in a DataFrame.

* Let's rename all the column names in our DataFrame which contain spaces in them. Also we will rename the column 'race/ethnicity' to 'race'.







![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_c549691d92c84a23b2202c20e0d13c20.png)






* We can get the list of all the columns using the attribute **`columns`**.





![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_e52bfb1ea5f64422891e14fa2afad24f.png)





![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_1dc745e4be2b45e3adaa8b279cb8be0e.png)





* We can also rename the indexes of the DataFrame using the rename() function as shown in the image below:

![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_55b82c3ed59e49438c8767bd019afe5b.png)


![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_9e61b169af2c4f9f8e9d9c8afc9b326e.png)