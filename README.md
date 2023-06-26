# Dog-Breed-Detection-Android

I have uploaded the file in Releases you can check this from tag button above.

# Abstract:
The "Dog Breed Detection" Android app uses a pre-trained machine learning model to classify dog breeds based on images. The app provides two options for input: capturing a photo using the device's camera or selecting an image from the gallery. After processing the image, the app displays the detected dog breed along with the confidence level of the prediction. The app utilizes the TensorFlow Lite framework for efficient and fast inference on mobile devices.


# Methodology:

# User Interface Design:

The app's main layout is implemented using a RelativeLayout, which allows for flexible placement of UI elements.
The layout consists of an ImageView to display the selected or captured image, two buttons for taking a picture or opening the gallery, and three TextViews for displaying the classification result.
Image Processing and Classification:

The captured or selected image is processed and prepared for input into the machine learning model.
The image is resized to a fixed size of 224x224 pixels using the Bitmap.createScaledBitmap() function.
The resized image is converted into a ByteBuffer, which is the expected input format for the TensorFlow Lite model.
The Classifier class handles loading the pre-trained model and labels from the app's assets folder.
The model and labels are loaded into memory during initialization using the AssetManager and FileInputStream.
The TensorFlow Lite interpreter is created using the loaded model file.
The classifyImage() function in the Classifier class performs the inference by running the input image through the interpreter.
The output of the model is processed to obtain the predicted dog breed and the corresponding confidence level.
User Interaction and Permissions:

The app requests the necessary camera permission at runtime using the ActivityCompat.requestPermissions() method.
When the user clicks the "Take Picture" button, the app opens the device's camera using an intent.
After capturing an image, the onActivityResult() method receives the result and extracts the image data as a Bitmap.
The captured image is then passed to the image processing and classification pipeline.
Similarly, when the user clicks the "Open Gallery" button, the app opens the device's gallery using an intent.
The selected image is retrieved and processed similar to the captured image.

![image](https://github.com/malikhadi09/Dog-Breed-Detection-Android/assets/92660593/3ee59558-2863-4ffc-93dc-8ba7b1d2b99b)

# Results:
The "Dog Breed Detection" app successfully integrates a trained machine learning model for classifying dog breeds. The app provides a user-friendly interface with options to capture photos or select images from the gallery. After the image is processed, the app displays the predicted dog breed along with the confidence level of the classification. The classification accuracy and performance depend on the quality of the pre-trained model and the input image. Further improvements can be made by utilizing more advanced machine learning models or by fine-tuning the existing model with additional data specific to the target use case.




 # Results and Discussion:

Present the results obtained from running the app and discuss their implications. Include sample images and corresponding classifications to showcase the app's accuracy. Analyze any limitations or challenges encountered during the development and usage of the app.
                
 ![image](https://github.com/malikhadi09/Dog-Breed-Detection-Android/assets/92660593/0d03a5b9-ecd4-4323-875f-378afb33b3c2)
![image](https://github.com/malikhadi09/Dog-Breed-Detection-Android/assets/92660593/b73b0ca0-bb7d-4eb2-985d-95870efdcb85)
![image](https://github.com/malikhadi09/Dog-Breed-Detection-Android/assets/92660593/20323b48-c55c-47d4-8a64-dd80743933ca)

                                  

# Conclusion:

The "Dog Breed Detection" app demonstrates the integration of machine learning models into Android applications for real-time image classification tasks. By leveraging the TensorFlow Lite framework and a pre-trained model, the app provides accurate predictions of dog breeds based on user-captured or gallery-selected images. The app's user-friendly interface and seamless interaction make it accessible and engaging for dog breed enthusiasts or anyone interested in dog identification. With further enhancements and refinements, the app can be extended to support additional features such as breed-specific information, image sharing, or multi-class classification for other objects or animals.


# Future Enhancements:

Provide suggestions for future improvements and enhancements to the app. Discuss possible avenues for extending the functionality, such as incorporating additional features, refining the classification algorithm, or exploring multi-class classification for other objects or animals.

