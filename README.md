# Newspaper-OCR-Project
Welcome to my project! I worked on this to be applied to the Michigan Daily, to be used to reformat old newspapers in the archives into the more modern format we use for online media. To accomplish this, I used Pytesseract, as well as OpenCV and Pillow for preprocessing the images of the archived newspapers and to morph it to make it more readable for the OCR algorithm. 

## Image-Preprocessing
The first step to completing this project was to preprocess and morph the images using OpenCV and Pillow to make it more readable for the OCR algorithm, Newspapers are messy, especially old ones, and are filled with random noise such as black bars that would largely affect the efficiency and accuracy of Pytessesract. To counteract this, I used OpenCV to morph the images into a way that the computer could detect white contours to draw bounding boxes around blocks of text in each individual newspaper. This way, only the text would be read in at first, seperate from all the margins, titles, and everything else. This will be tuned more and used in the future to extract the headline and first paragraph from each paper to display with a "Read More" option on the main website.

The Image Preprocessing Process is Displayed Below:
### Original Image
<img width="453" alt="Screenshot 2024-01-17 at 3 56 08 PM" src="https://github.com/MathewZheng/Archived-Newspaper-OCR-Processing-Analysis---Michigan-Daily/assets/53542045/7ed7346c-40f7-4242-8fc3-e0b0f6d4e20a">

### Greyscale and Slight Blur
<img width="455" alt="Screenshot 2024-01-17 at 3 55 47 PM" src="https://github.com/MathewZheng/Archived-Newspaper-OCR-Processing-Analysis---Michigan-Daily/assets/53542045/4492a055-4333-4b07-9e54-d0c178910774">

### Image Binirization by Applying Threshhold
<img width="451" alt="Screenshot 2024-01-17 at 3 58 05 PM" src="https://github.com/MathewZheng/Archived-Newspaper-OCR-Processing-Analysis---Michigan-Daily/assets/53542045/5b588fd4-0ea9-45cf-86ee-03e31c5b5881">

### Dilation
<img width="451" alt="Screenshot 2024-01-17 at 3 58 27 PM" src="https://github.com/MathewZheng/Archived-Newspaper-OCR-Processing-Analysis---Michigan-Daily/assets/53542045/84a3675d-cea3-4385-b640-2598f81fc5c4">

### Detecting Countours and Creating Visible Bounding Boxes
<img width="492" alt="Screenshot 2024-01-17 at 3 56 34 PM" src="https://github.com/MathewZheng/Archived-Newspaper-OCR-Processing-Analysis---Michigan-Daily/assets/53542045/cae5f1a9-1df5-40f7-96d8-c8e92028d2f2">
