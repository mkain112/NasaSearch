# Nasa Search

While attempting to use the NASA images API to collect images for a machine learning application I discovered that simple search for 'planet' I conducted did not return a good sample of planets. There were many intermixed images of NASA ground operations and Community outreach event. I decided to attempt to use computer vision to sort the 'planets' from 'not planets' instead of attempting to refine my API search. This became a project in its own right.

## Getting Started

These ipython notebooks will get you a copy of the code up and running on your local machine for development and testing purposes. You will have to pull your own images and sort them into planet/not planet or whatever Boolean pair you decide to use, I have not yet stored the images or completed model on GitHub (files are too large).

### Prerequisites

Use the Space EDA notebook to scrape images from the NASA API or use it as a template for gathering images from other sources.

You will have to have the images sorted into categories and stored in directories reflecting those categories to use this code without major modification.
![alt text][planetornot]

### Results

The first model constructed is a simple Sequential CNN trained on around 1200 images. 
![alt text][FirstModel]

The second model uses transfer learning with the Vgg16 CNN, which is trained on all of the images on ImageNet.
![alt text][vgg16Model]

## Built With

* [NASA API](https://api.nasa.gov/) 
* [Vgg16](https://keras.io/api/applications/vgg/#vgg16-function) – Keras source for the Vgg16 model

## Slideshow

* [GoogleSlides](https://docs.google.com/presentation/d/1dZp84LE8ghdW0R4i--vkRscxogsvKhGNatiOdvxWg1E/edit?usp=sharing)


[FirstModel]: https://github.com/mkain112/NasaSearch/blob/master/Images/CNN%20to%20classify%20NASA%20images%20(3).jpg?raw=true 
[vgg16Model]: https://github.com/mkain112/NasaSearch/blob/master/Images/CNN%20to%20classify%20NASA%20images%20(4).jpg?raw=true
[planetornot]: https://github.com/mkain112/NasaSearch/blob/master/Images/CNN%20to%20classify%20NASA%20images%20(1).jpg?raw=true
