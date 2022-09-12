# Semantic Segmentation of the lungs from X-ray images
A model of the segmentation of the lung region from the x-ray images, the model relies on forming a mask through which that region can be cut.
- The methodology that was followed to build the model, depends on the use of a pre-trained model, to extract the characteristics from it, and then rely on those characteristics and train them to find a mathematical formula that links these characteristics to each other and thus the ability to build the mask as required.
The following images show the characteristics of one of the X-ray images, which were extracted from the previously trained VGG19 model, where the layer to be extracted from the features was selected.
![download (74)](https://user-images.githubusercontent.com/108609519/189716915-e0d21298-bc62-46b4-bfd7-4c1f53ed10a9.png)

- In the next stage, all the images will be passed to the previous model to get the attributes for each attribute, from which the required dataset is formed.
- The methodology is based on that the sum of the attributes of each pixel corresponds to the value of the pixel in the mask image, and therefore each pixel of the mask image (TARGET) corresponds to 64 attributes of the corresponding pixel value of the X-ray image.
# Results:
## The following diagrams show the results obtained for the training data and the test data.

![download (75)](https://user-images.githubusercontent.com/108609519/189717090-2df5c99b-52c7-42c7-9e0a-07481723f33a.png)
![download (76)](https://user-images.githubusercontent.com/108609519/189717126-2593ec89-6edf-4020-b5b9-5737252af71b.png)

## The model has been tested on a number of images:

![image](https://user-images.githubusercontent.com/108609519/189717435-1645197e-176a-441d-bdc3-49d83d8f4acf.png)
![image](https://user-images.githubusercontent.com/108609519/189717966-655d0a42-3461-4a8f-bcd0-e6847e33140c.png)
![image](https://user-images.githubusercontent.com/108609519/189717720-267c8146-04d6-46ad-93ce-a35bf054d188.png)
![image](https://user-images.githubusercontent.com/108609519/189718276-ea69ce44-a203-4350-81de-1ae40281077a.png)



