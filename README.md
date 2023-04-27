# What-number-is-this-Hopfield-Neural-Network

This project is a Hopfield Neural Network implemented in Matlab for recognizing handwritten numbers. The network is trained on a set of 32x32 images of handwritten numbers and can reconstruct distorted or incomplete patterns. but it also have the capacity to get its training data from a selected folder.

## Demo
![Gif Numero 3 reconociendoce](https://user-images.githubusercontent.com/107207740/234096137-c1c36f81-5785-4186-a909-e1ad89e70cae.gif)

## Installation
* Clone this repository: git clone https://github.com/CristianLav/What-number-is-this-Hopfield-Neural-Network
* Open Matlab and navigate to the cloned repository directory
* Run Hopfield_UI.mlapp to start the application

"Note: to upload an image, it must be in the same folder as the Hopfield_UI.mlapp file, otherwise the program won't be able to recognize the image."

## Usage
The application can be used to recognize handwritten numbers. To recognize a number:

* Select the desired method for the Holfield algorithm (Hebbiano , PseudoInversa).
* Click "Entrenar" a window will appear asking you to select a folder. This folder must contain all the datasets required for recognition.
* Afterward, click on "Cargar Patrón", and a window will appear prompting you to select an image. Please note that the image you select must be the same size as the dataset image, and it should be located in the root directory of the project. Also it only have been tested  with black and white images
* if done correctly your image will be display in the app.
* The "Manual" button is used to draw an 8 by 8 pattern, and it only works when the network has been trained with an 8 by 8 dataset..
* After the image has been successfully uploaded, the noise slider can be used to distort the image. However, if the image is large, this may take a while to apply the distortion.
* To choose between asynchronous and synchronous modes, select the 'Funcionamiento' field. This determines how the matrix will collapse to recognize the pattern. Please note that the asynchronous mode has a built-in delay, which can be seen in the videos and can add to the overall user experience.
* Finally, click on the 'Reconocer' button for the system to recognize the pattern.


## Dataset
The dataset used to train the network is included in the data folder. It contains just 10 32x32 images of handwritten numbers, made in paint, and another folder of 3 8x8 image.



## Usage Examples

One way that the system can perform internal calculations is by using either the Hebbian or PseudoInverse method. The demo video shows the PseudoInverse method, but the operation in Hebbian mode is also available, and the visualization is nearly identical. Additionally, if the noise is too high, the system may recognize the negated form of the pattern.

![GIf Numero 9 Reconociendoce](https://user-images.githubusercontent.com/107207740/234096168-26965786-6d25-41b4-9bfa-427dd9eb7c57.gif)


As mentioned earlier, the asynchronous method has a delay built into it, which allows for the cool animations to be seen. On the other hand, the synchronous method shows the actual speed of recognition without delay.

![Gif 8 Reconocido Real Speed](https://user-images.githubusercontent.com/107207740/234096234-99618923-5a4c-4e4d-a24d-40c81501cd37.gif)


The system can recognize the same pattern with a higher degree of noise, which may show the negated form of the 8 pattern.

![Gif 8 negado Reconocido Real Speed](https://user-images.githubusercontent.com/107207740/234096296-b8d66ab3-cefb-4586-b0be-f1e55839c91a.gif)
