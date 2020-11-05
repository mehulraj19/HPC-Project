# HPC-Project
Covid 19 detection using chest X-rays

<h1>Introduction</h1>
The project covers very important aspect in the sitatuation we are in and has been developed keeping in mind to actually help the frontline warriors, the doctors, to speed-up the
diagnosis process. Supervised Learning is been used while training the model. Machine Learning can be used for prediction and classification, but when we are talking about datasets
having images, a part of ML, Deep Learning, can bes used effectively for these training models. the dataset can be found <a href="https://www.kaggle.com/tawsifurrahman/covid19-radiography-database">here</a>. 

<h1>Working</h1>
Here, the model has been trained using the concepts of Deep Learning and Image Pre-Processing in mind. The model has been developed keeping two important things in mind:
<ul>
  <li><ins>Model must have high accuracy</ins> since the model is actually developed for medical purposes therefore it is important to have good precesion for giving results.</li>
  <li><ins>The computational cost must be keep in check</ins> so that one can actually get the results in less time but this must not affect accuracy.</li>
</ul>

<h1>Model</h1>
Model working is divided into phases:
<ol>
  <li>
    <h2>Data Pre-Processing (Image Pre-Processing)</h2>
    <ul>
    <li>
    <ins><h4>RGB to Gray-Scale</h4></ins>
    The dataset contains images that have RGB effect. Now, when we actually want to reduce computational cost, we can actually recieve this via reducing RGB to Gray-Scale. Now, 
    it is important to note that this can not actually be done for all the models, here color of the image does not plays any role, therefore, we can remove this.
    </li>
    <li>
    <ins><h4>Standardizing Image Size</h4></ins>
    Standardizing image size is important step since different image size will bring out features after CNN, that may not be useful at all for the model prediction, therefore it is
    is the important step to perform before starting with model training.
    </li>
    </ul>
  </li>
  <li>
  <h2>Model Layers CNN</h2>
  Convolutional Neural Network (CNN) is widely used for image classification. the model actully works well for the working that we desire in this project. The model has been 
  developed with 4 layers, three of them are for input layers and one for output layer. 'relu' as activation layer is used in internal working, 'sigmoid' activation layer is 
  used for output layer. 
    <br/><ins>'relu' activation layer</ins>: Here, it takes positive value as it is if the model is giving it, and if we are getting negative value from model, it will assign the value for 
  that to be 0. That is the reason it is referred as rectified networks.
  <br/><ins>'sigmoid' activation layer</ins>: Since, we can have value only 0 or 1 (bipolar outputs), therefore, we need to make sure that we are taking care of values that comes
  in between [0,1]. Normally , value < 0.5 is taken as 0 and values > 0.5 is taken as 1.
  </li>
</ol>

<h1>Results</h1>
The model has been developed quite well.
<br/> Validation accuracy: 98.38%

<h1>Conclusions</h1>
Overall, I got the chance to take a dive in Deep Learning, and I have found really challenging and iteresting at the same time. The model trained is actually working well and
the computational cost has been reduced greatly after doing the Data Pre-Preprocessing. The project actually covers most of the aspects of Data Science and I have found all this
really interesting.
