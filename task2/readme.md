# Task2-Margi_Pandya

# Problem Statment:
Topic 2
- Basic Image classifier CNN
-  So Neural Nets are your go to approach for solving any problem.
-  Create a labeled dataset of Avengers images- Captain America, Iron Man,Black Widow, Hulk,Thor. (Try ​scraping ​images from internet , instead of manually creating the dataset)
-  Train a CNN that is able to classify an unseen image with reasonable accuracy.
-  You can use frameworks like ​PyTorch​ and ​Keras ​to simplify your workflow.


## Convolutional Neural Networks - Plan of Attack
### Step 1: Convolution Operation
  #### Step 1(b): ReLU Layer
#### Step 2: Pooling
### Step 3: Flattening
### Step 4: Full Connection


### What is convolution?
 Expresses how the shape of one is modified by the other.
 ![image](https://user-images.githubusercontent.com/117746681/202832707-947036e1-14e7-49d6-90ed-8a6f5097010d.png)

### How exactly does the convolution operation work?
You can think of the feature detector as a window consisting of 9 (3x3) cells. Here is what you do with it:

1. You place it over the input image beginning from the top-left corner within the borders you see demarcated above, and then you count the number of cells in which the feature detector matches the input image.
2. The number of matching cells is then inserted in the top-left cell of the feature map.
3. You then move the feature detector one cell to the right and do the same thing. This movement is called a and since we are moving the feature detector one cell at time, that would be called a stride of one pixel.
4. What you will find in this example is that the feature detector's middle-left cell with the number 1 inside it matches the cell that it is standing over inside the input image. That's the only matching cell, and so you write "1" in the next cell in the feature map, and so on and so forth.
5. After you have gone through the whole first row, you can then move it over to the next row and go through the same process.

![image](https://user-images.githubusercontent.com/117746681/202832792-a9f936ee-775b-4da7-a429-2f2fcb40a598.png)

### ReLU 

![image](https://user-images.githubusercontent.com/117746681/202832867-ccd9618e-4883-4c77-923f-f5e0abc47bad.png)
The purpose of applying the rectifier function is to increase the non-linearity in our images.

### Max Pooling
Max pooling is concerned with teaching your convolutional neural network to recognize that despite all of these differences that we mentioned, they are all images of cheetah.
![image](https://user-images.githubusercontent.com/117746681/202833349-3650897d-9b15-44ac-aa8d-f982fb01f8eb.png)

### Flattening
![image](https://user-images.githubusercontent.com/117746681/202833386-1c62a9dc-891c-42d7-aaad-0828d22a2235.png)
As the name of this step implies, need to flatten the pooled feature map into a column like in the image below.

### Full Connection
1. Input layer
2. Fully-connected layer
3. Output layer
![image](https://user-images.githubusercontent.com/117746681/202833448-b4a46973-e754-4cd1-bc5f-bbf1391106a4.png)



