# AUTOMATIC LICENCE PLATE RECOGNITION MODEL
This Automatic Licence Plate Recognition Model was created using OpenCV and Pytesseract using Python as the core programming language.
And Jupyter Notebook was used as the IDE for creation of this model.

The model takes in the image of a vehicle as shown in the below example

![image](https://user-images.githubusercontent.com/77007539/129399329-ab343ea6-465e-452d-aca4-3c1dab0dfd0c.png)

The image is converted into the gray image at the first step itself.

Then a bilateral filter is applied to the image to take a note of the boundaries and lines present in the image as shown below

![image](https://user-images.githubusercontent.com/77007539/129399462-7cbe94bc-c991-4e33-802a-db088e82a62a.png)

After the bilateral filter, the image is further applied with contouring and masking specifying the approx. co-ordinates of the licence plate in the image 

and then the rest of the image is masked out and only the licence plate remains

![image](https://user-images.githubusercontent.com/77007539/129399595-85d1993e-13e1-4c1e-a2da-afe9671394f9.png)

After the masking is done, it is easier to crop the image around the licence plate to get a better look at it.

![image](https://user-images.githubusercontent.com/77007539/129399660-d204c017-ded8-48ec-8c82-10ce77273798.png)

After this the image is put under the TesseractEngine to extract the registration Number from the image and also the state it belongs to

![image](https://user-images.githubusercontent.com/77007539/129399749-524a2b31-3a07-46c3-afa0-15f5013dfdcf.png)
