# What is Machine Learning?

![](http://vignette4.wikia.nocookie.net/uncyclopedia/images/e/e3/Arnold_governator.jpg/revision/20070220123156)

[Excellent video source where I got most of my info](https://www.youtube.com/channel/UC_x5XG1OV2P6uZZ5FSM9Ttw)






## How would you write code that returns if an image is an apple or orange?

![](http://juliandance.org/wp-content/uploads/2016/01/RedApple.jpg)
![](https://goo.gl/images/glfCKa)
- count color pixels? 
- map outline points and compares to hard coded image maps?


Now you get a black and white image or a picture with no fruits at all!
###A banana just broke your code...

Before you get to tackle this bug, I want your program to also tell the difference between cats and dogs





##Lets train a Classifier aka function

A classifier crams data (trait) into the sausage machine that assigns it a label 

> ex: apple / orange   or   email as spam / not spam
	this is called classified learning 

[SciKit Learn](http://scikit-learn.org/stable/install.html) provides many datasets to play with that are easy to import
[with Anaconda dependancies](https://www.continuum.io/downloads)





## Now for training data
- ### Real world: this is called data collection. 
- ### Machine learning: these are called >features

> ex: weight, texture, height...

and these are best as booleans (0 for bumpy, 1 for smooth)




### CODE:
- `.DecisionTreeClassifier()` is an algorithm that identifies patterns 
- `.fit()` finds patterns in data
- `.predict([[160,0]])` returns the prediction based on 160g and bumpy




##Types of classifiers
- ![Artificial Neural Network](https://goo.gl/images/D4EC4r)
- ![Support Vector Machine](https://goo.gl/images/H1ghsj)
- ![Decision Tree](https://goo.gl/images/27IDKR)
- ![k-nearest neighbors](https://goo.gl/images/P35wev)

For k-nearest neighbor:
-Euclidean Distance (similar to a^2+b^2=c^2)
-works in more than 2d >> 3d,4d... mind melting in 5d+

![](http://www.tenthdimension.com/medialinks.php)




###[Playground!](http://playground.tensorflow.org/?utm_campaign=ai_series_pipeline_051116&utm_source=gdev&utm_medium=yt-desc#activation=tanh&batchSize=10&dataset=circle&regDataset=reg-plane&learningRate=0.03&regularizationRate=0&noise=0&networkShape=4,2&seed=0.96356&showTestData=false&discretize=false&percTrainData=50&x=true&y=true&xTimesY=false&xSquared=false&ySquared=false&cosX=false&sinX=false&cosY=false&sinY=false&collectStats=false&problem=classification&initZero=false&hideText=false">playground)






##Image classifiers
[TensorFlow for Poets](https://goo.gl/QTwZ3v) uses a neural network to train classifier with seeded images(~100)

- deep learning to determine features from code instead of hard coding (this example used pixels)
-the more diversity and quantity of images increases the accuracy of prediction
- ####Fun Fact:#### Google's Inception image classifier trained on 1.2 million images took 2 weeks to execute


[handwritten number machine learning](https://www.youtube.com/watch?v=Gj0iyo265bc)

