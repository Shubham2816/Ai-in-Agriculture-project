# Ai-in-Agriculture-project : A Report

ABSTRACT

INFO :

Plant diseases and pests are important factors determining the yield and quality of plants. Plant diseases and pests identifcation can be carried out by means of digital image processing. 

In recent years, deep learning has made breakthroughs in the feld of digital image processing, far superior to traditional methods. How to use deep learning technology to study plant diseases and pests identifcation has become a research issue of great concern to researchers. This review provides a defnition of plant diseases and pests detection problem, puts forward a comparison with traditional plant diseases and pests detection methods. According to the diference of network structure, this study outlines the research on plant diseases and pests detection based on deep learning in recent years from three aspects of classifcation network, detection network and segmentation network, and the advantages and disadvantages of each method are summarized. 

Common datasets are introduced, and the performance of existing studies is compared. On this basis, this study discusses possible challenges in practical applications of plant diseases and pests detection based on deep learning. In addition, possible solutions and research ideas are proposed for the challenges, and several suggestions are given. 

Finally, this study gives the analysis and prospect of the future trend of plant diseases and pests detection based on deep learning. 
INTRODUCTION


Plant diseases and pests detection is a very important research content in the field of machine vision. It is a technology that uses machine vision equipment to acquire images to judge whether there are diseases and pests in the collected plant images .
 At present, machine vision-based plant diseases and pests detection equipment has been initially applied in agriculture and has replaced the traditional naked eye identification to some extent. For traditional machine vision-based plant diseases and pests detection method, conventional image processing algorithms or manual design of features plus classifiers are often used . This kind of method usually makes use of the different properties of plant diseases and pests to design the imaging scheme and chooses appropriate light source and shooting angle, which is helpful to obtain images with uniform illumination. 
Although carefully constructed imaging schemes can greatly reduce the difficulty of classical algorithm design, but also increase the application cost. At the same time, under natural environment, it is often unrealistic to expect the classical algorithms designed to completely eliminate the impact of scene changes on the recognition results .
 In real complex natural environment, plant diseases and pests detection is faced with many challenges, such as small diference between the lesion area and the background, low contrast, large variations in the scale of the lesion area and various types, and a lot of noise in the lesion image.

Also, there are a lot of disturbances when collecting plant diseases and     pests images under natural light   conditions. 




At this time, the traditional classical methods often appear helpless, and it is difficult to achieve better detection results. 

In recent years, with the successful application of deep learning model represented by convolutional neural network (CNN) in many fields of computer vision (CV, computer-vision), for example, traffic detection , medical Image Recognition , Scenario text detection, expression recognition , face Recognition [, etc. Several plant diseases and pests detection methods based on deep learning are applied in real agricultural practice, and some domestic and foreign companies have developed a variety of deep learning-based plant diseases and pests detection WeChat applet and photo recognition APP software. Therefore, plant diseases and pests detection method based on deep learning not only has important academic research value, but also has a very broad market application prospect

In view of the lack of comprehensive and detailed discussion on plant diseases and pests detection methods based on deep learning, this study summarizes and combs the relevant literatures from 2014 to 2020, aiming to help researchers quickly and systematically understand the relevant methods and technologies in this field. The content of this study is arranged as follows: “Definition of plant diseases and pests detection problem” section gives the definition of plant diseases and pests detection problem; “Image recognition technology based on deep learning” section focuses on the detailed introduction of image recognition technology based on deep learning; “Plant diseases and pests detection methods based on deep learning” section analyses the three kinds of plant diseases and pests detection methods based on deep learning according to network structure, including classification, detection and segmentation network; “Dataset and performance comparison” section introduces some datasets of plant diseases and pests detection and compares the performance of the existing studies; “Challenges” section puts forward the challenges of plant diseases and pests detection based on deep learning; “Conclusions and future directions” section prospects the possible research focus and development direction in the future. 
IMAGE RECOGNITION TECHNOLOGY BASED ON DEEP LEARNING

  Compared with other image recognition methods, the image recognition technology based on deep learning does not need to extract specific features, and only through iterative learning can find appropriate features, which can acquire global and contextual features of images, and has strong robustness and higher recognition accuracy.

Deep learning theory the concept of Deep Learning (DL) originated from a paper published in Science by Hinton et al. in 2006. The basic idea of deep learning is: using neural network for data analysis and feature learning, data features are extracted by multiple hidden layers, each hidden layer can be regarded as a perceptron, the perceptron is used to extract low-level features, and then combine low-level features to obtain abstract high-level features, which can significantly alleviate the problem of local minimum.

Deep learning overcomes the disadvantage that traditional algorithms rely on artificially designed features and has attracted more and more researchers’ attention. It has now been successfully applied in computer vision, pattern recognition, speech recognition, natural language processing and recommendation systems . Traditional image classification and recognition methods of manual design features can only extract the underlying features, and it is difficult to extract the deep and complex image feature information . And deep learning method can solve this bottleneck. 

It can directly conduct unsupervised learning from the original image to obtain multi-level image feature information such as low-level features, intermediate features and high-level semantic features. Traditional plant diseases and pests detection algorithms mainly adopt the image recognition method of manual designed features, which is difficult  and depends on experience and luck, and cannot automatically learn and extract features from the original image


At present, deep learning methods have developed many well-known deep neural network models, including deep belief network (DBN), deep Boltzmann machine (DBM), stack de-noising autoencoder (SDAE) and deep convolutional neural network (CNN).  

CNN in computer vision tasks have boosted the growing popularity of deep learning. In the convolution layer, a convolution core is defned frst. Te convolution core can be considered as a local receptive feld, and the local receptive feld is the greatest advantage of the convolution neural network. When processing data information, the convolution core slides on the feature map to extract part of the feature information. After the feature extraction of the convolution layer, the neurons are input into the pooling layer to extract the feature again. At present, the commonly used methods of pooling include calculating the mean, maximum and random values of all values in the local receptive field.

