# Dance-Form-ML
Model to classify Dance Style from various Indian Dance Forms.

You can get dataset from [here](https://www.kaggle.com/somnath796/indian-dance-form-recognition?)
1. Data Preprocessing:
	I converted the input training images to the size of 128X128.
	Then converted Categories in to classes from 0 to 7 and then converted them to one-hot-encodings.
2.Model:
	I keras Sequential model for training.
	The fist layer is Conv2D layes with  kernel size=(3,3) and "relu"(rectified linear unit) activation function and a maxpooling layer
	Then two similar layers with diferent number of convolutions.
	These layers give output in 3D format and to change them to 1D array a flatten layer is used.
	Then one fully connected Dense layer with "relu" activation fucntion
	Now to manage overfitting we use DropOut
	Then in last one Dense Layer with Softmax activation
This model is compiled using categorical crossentropy loss function 
	
