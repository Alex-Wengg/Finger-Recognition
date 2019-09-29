Data Organized and Labeled for Object Detecting: #https://www.dropbox.com/sh/3ynzwzksoh5yr03/AAAMSuoow01X-A9Myth3ocnXa?dl=0

The Module Used for Training and Testing: https://github.com/tensorflow/models/research/object_detection

This was an attempt at TensorFlow object detection, it took three trials of data reorganizing. Using LabelImg to label the location of the objects to detect on the image. Each trial, more images were added to increase the accuracy and consistency of the, by the end about 500 images of testing and training were used to train the model. A majority of the time was taken to gather diverse sets of images, for example, images with different shades of backgrounds and objects at different angles. A finger tilted at a 45 degree on a white background. The previous 2 trials would only work in darker backgrounds with little light sources to work with some degree of accuracy.

This project took 3 weeks to train, mostly due to configuring the required modules and data gather and organizing. Another problem was the demand for a stronger GPU and ram to run the training without technical difficulty. The first trial was trained for 10 minutes and 50 images on a Mac with 8 GB 1600 MHz DDR3 memory and it threw off the screen display with red, green and blue lights flashing over the screen. The solution was to use a cloud GPU, for this case it was Paperspace at the price of 0.50 cost per hour, charged when the machine is activated.

Even with about 500 images, the model still had trouble finding 60% confidence in object detecting but when the threshold is lowered to 10%, it was effective at recognizing the desired object in the video with no misidentifying. It didn't mistake a pencil for a finger or any other sound.

The code for this doesn't include how to train another object detector but just the files that were trained and setups to use the camera image recognition. There are many other sources and tutorial used to train another object detector such as

https://github.com/EdjeElectronics/TensorFlow-Object-Detection-API-Tutorial-Train-Multiple-Objects-Windows-10

and

https://pythonprogramming.net/training-custom-objects-tensorflow-object-detection-api-tutorial/?completed=/creating-tfrecord-files-tensorflow-object-detection-api-tutorial/

This was just a personal projection tensor object detection model, future progress is uncertain as TensorFlow is a massive and complicated library to use without much understanding. University work may also limit my time to work on it and even other interests will most likely distract me from making future work to build upon this model.

And lack of evidence for the work done on this was due to using a Cloud GPU, essentially a virtual machine, lack of knowledge for using Github and forgetting due to mismanagement by my part.
