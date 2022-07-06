# Series

## Learning Objectives

* What is Series?
* Create a Series

## Pandas Objects

Before we dive into series, let’s do a quick recap of pandas ‘objects’. At the core of the pandas library, there are two fundamental data structures/objects:

* Series
* Data Frames

## What is a Series?

* A one-dimensional labeled array
* Can hold data of any type
* Is like a column in a table

## What can a Series have?

* A Series can have all the elements as numbers in it:






![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_d0cedac8c4d14c8c9655af50c4da5baa.png)






* A Series can have all the elements as strings in it:



![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_fdc09c325d12430db04f51d5184055eb.png)



* A Series can have its elements as both numbers and strings. 
* But the data type of the Series is always ‘object’ in this case:




![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_c009b262e19442bcba27b0443b9df483.png)




* Series is like a list in Python which can take any type of value like integers, strings, floats (or decimal values), etc.
* All the items in series are labeled with indexes:




![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_93dd761ed388443fbf91ccb17b94fecb.png)




* **By default indexing starts from 0 in Series.** 

## **Human vs Python Index**

* Indexes that we (Human) understand:


![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_7f29921bb6fe4d89805e73bde9c929ba.png)


* Indexes that Python understands:



![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_1e0299f3ee16440597df44913e70aba8.png)



**Well, it all starts with ‘0’. That’s the only difference.**

## Create a Series

* Remember to import the library before using it!

  **`import pandas as pd`**

* You can create your own Series using a Python list:





![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_b065378a1c3b4c20990cb7a4fc825d2b.png)





* You can also create your own Series using a dictionary:

![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_937099e6513a4788ae90cbaf8c6bb80d.png)