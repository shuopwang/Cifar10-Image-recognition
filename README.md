# Cifar10-Image-recognition
After reading the Ng's article &lt;single layer networks in unsupervised feature learning>. The paper is published in 2011. I try to practice this project.

All the codes are writen in Jupyter Notebook, so you guys could see the result clearly.

The naif K-means is just using the K-means to cluster the image, and see the result. Just for fun.

The version 1 there is something i wrongly unstood, but i will still poster. 

The version 2, I got the good result. The basic idea of this article is following, for n*n patch do a K-means clustering, to get the hidden label. Then try to create dictionary for both the train and test image. Finally, using the standard classification model like SVM to do the classification. This idea quite like the bag-of-words in the image processing. The difference is that, in the normal way, we cluster those feature, howerver in this article we do the cluster for the patch.  

The first is the soft dictionary, which means in the E step, we don't force the data belongs to the closest class, but using the probability to measure the relation.  

The second is the hard dictionary, just standard K-means.    
 
I use the SVM to be the final classification as Ng suggest in the article.  

Also, after 6 months, I try this simple task with Pytorch, expericement with VGG-16 and the CNN network of my own.   
