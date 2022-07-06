# Basic Methods & Attributes of DataFrame


## Dataset: Exam Scores

This dataset contains marks secured by different students in an examination and their background information.

The dataset can be found here:

* [https://github.com/dphi-official/Datasets/blob/master/exam_scores.csv](https://github.com/dphi-official/Datasets/blob/master/exam_scores.csv)


## Read The dataset

* So far you have learned how to read a csv file using read_csv() function. Let’s see the practical implementation.
* read_csv() function is of pandas library. So the first task is always to import/load the library we will use.

![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_961186b0348e4d039253c2c1d82e96be.png)

* To read a csv file, use read_csv() function of pandas library.

![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_fc122795984a40bab02c4807bb7e16ac.png)
* **The csv file ‘exam_scores’ is located in the current working directory.**

## Methods and Attributes of DataFrame

### shape attribute

* **shape:** It will help you to know what is the shape of your DataFrame, i.e., (number of rows, number of columns).
* After we have loaded the data we can check the shape of the DataFrame this attribute:


![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_73cf0373a3694991b6b3ba2456b79332.png)


* So our DataFrame has 1000 rows and 8 columns. From here, we can also say that our DataFrame has 8000 entries.

### head( ) method

* **head( ):** It will help you see the first five observations of your DataFrame. You can get some idea about the content of your DataFrame.
* head() gives us a quick look at the contents of the DataFrame, like column headers, data types of columns, what data each column has, etc.




![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_94b9687ad8894e35b64068ff71ec7e7b.png)




* **We can see the first five observations of the dataset in the above table.**

### tail( ) method

* **tail( ):** This method is similar to head() method but instead of first five it will give you the last five observations from your dataset.




![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_6af2f3f996e248c19b8ca028c923b893.png)



* **We can see the last five observations of the dataset in the above table.**

### head( ) and tail( )

We can also add the number of rows to be displayed in both head( ) and tail( ). See the examples below:



![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_bf7d9c12197442089d79254cd673b18e.png)


### dtypes

* **dtypes:** It will help you know about the data types of each column.
* To know the data types associated with each column, we can use dtypes attribute.







![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_f485545ea6e947f786a14f24169f310f.png)





We can observe from this output:

* 'gender', 'race/ethnicity', 'parental level of education', 'lunch' and 'test preparation course' are of data type - object.
* 'math score', 'reading score' and 'writing score' are of data type - int64 (i.e. integer).

### info( )

* **info( ):** This method will return a concise summary about the DataFrame.







![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_3a44a0fb5bb94f5b89a06cdafab34ed3.png)






**What do you get using info()?**



![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_79f5d0520ee04e1fa58476f3c5264745.png)



As you can see, info() gives you a lot of different information about the DataFrame, and can be quite useful!