## COMP431: Computer Vision Project  [ 2018-2019 AGU ]

In this project, computer vision feature matching is applied in order to find related product on market shelves image dataset. 


### Experimental Results
#### a) How many products are correctly found (#correct detections)?
I have collected shelf images from 5 different shelves and when I applied, SIFT, HOMOGRAPY and perspective transform to target and search image. I have correctly found all of them, since there should be 2 search product for each category, I correctly found 10 products. (all of them.)The results of the algorithm is already shown above. There is no doubt that while working such a project I had to re-watch Udacity course on sift, homography and perspective transform.

#### b) How many miss-detections did you get?
There is no miss detection in my dataset, I did NOT accidently found another product than searched one. It can also be observed from results of the algorithm above.

#### c) How many false detections did you get?
None.

#### d) Give numbers and ratios for each search item. Discuss your results. Explain why did you get those results for the best/the worst search.

__Category 1__

  - Product 1 > matched perfectly (%100)
  - Product 2 > matched perfectly (%100)

__Category 2__

  - Product 1 > matched perfectly (%100)
  - Product 2 > matched perfectly (%100)

__Category 3__

  - Product 1 > matched perfectly (%100) (Although there are less interest points compared to others, algorithm is performed very well.)

  - Product 2 > matched perfectly (%100)

__Category 4__

  - Product 1 > matched perfectly (%100)
  - Product 2 > matched perfectly (%100)

__Category 5__

  - Product 1 > matched perfectly (%100)
  - Product 2 > matched perfectly (%100) (Although the product is not clear in shelf image, the algorithm is performed very well. )

The main reason of getting best search results is understanding how an image can differentiate between each other, as well as, understanding of SIFT, Homograpy and perspective tranform operations. Besides, I tried to give importance on taking pictures at enough distance (not too away or not too close) and not including shadows ( which might require extra filtring techniques to implement.)

### Challanges

The main challenge was building required enviroment, I have tried different techniques and algorithms on feature matching. However when I started to try SIFT algorithm using OpenCV, the problems started seriosly, since SIFT algorithm is available in lower versions of OpenCV and another branch of OpenCV, I had to solve this problem on my local computer. Yet, I could not deal with it on my local computer because it requires reliable and fast internet connection, for this reason at the end of my hopes, I decided to use Cloud Computing, I have rent 30 GB Memory, 8 Core and 100 GB SSD server from Google. Then, I configured machine according to my desire to solve this problem, I install following OpenCV libraries to get access SIFT algorithm :

```

pip install opencv-contrib-python==3.4.2.17

pip install opencv-python==3.4.2.17

```
When those packages are installed correctly, my problem is solved on getting access to SIFT algorithm.

Another challange was learning homograpgy and perspective transform in order to draw encircle around the product on shelf images. So, I have spent a lot of time on watching Udacity course and searching way to complete this challenge. Finally, I understood how it works and why it is required, then I wrote the implementations.


### Example Market Shelves- 1 

![alt text](https://raw.githubusercontent.com/ahmetturkmen/CV-P1-2019-2020/master/data_/shelves/m1_shelf.jpg)


### Example Market Shelves- 2 

![alt text](https://raw.githubusercontent.com/ahmetturkmen/CV-P1-2019-2020/master/data_/shelves/c1_shelf.jpg)


### Example Market Shelves- 3 

![alt text](https://raw.githubusercontent.com/ahmetturkmen/CV-P1-2019-2020/master/data_/shelves/t1_shelf.jpg)



### Product to be searched on example market shelves- 1 

![Product 1- Example ](https://raw.githubusercontent.com/ahmetturkmen/CV-P1-2019-2020/master/data_/products/c2_product.jpg)


### Product to be searched on example market shelves- 2 

![Product 2- Example](https://raw.githubusercontent.com/ahmetturkmen/CV-P1-2019-2020/master/data_/products/c1_product.jpg)


### Product to be searched on example market shelves - 3 

![Product 3 - Example ](https://raw.githubusercontent.com/ahmetturkmen/CV-P1-2019-2020/master/data_/products/t1_product.jpg)


## Results

![Results-1 ](https://raw.githubusercontent.com/ahmetturkmen/CV-P1-2019-2020/master/results/result_1.png)

![Results-2 ](https://raw.githubusercontent.com/ahmetturkmen/CV-P1-2019-2020/master/results/result_2.png)

![Results-3 ](https://raw.githubusercontent.com/ahmetturkmen/CV-P1-2019-2020/master/results/result_3.png)

![Results-4 ](https://raw.githubusercontent.com/ahmetturkmen/CV-P1-2019-2020/master/results/result_4.png)

![Results-5 ](https://raw.githubusercontent.com/ahmetturkmen/CV-P1-2019-2020/master/results/result_5.png)



