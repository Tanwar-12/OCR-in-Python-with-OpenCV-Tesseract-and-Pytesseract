# OCR in Python with-OpenCV Tesseract and Pytesseract

### Preprocessing of images using OpenCV

*Basic functions for different preprocessing methods*
- grayscaling
- thresholding
- dilating
- eroding
- opening
- canny edge detection
- noise removal
- deskwing
- template matching. 

**Different methods can come in handy with different kinds of images.**

### Bounding box information using Pytesseract

**While running and image through the tesseract OCR engine, pytesseract allows you to get bounding box imformation** 
- on a character level
- on a word level
- based on a regex template

**We will see how to obtain all of them.**

### Page Segmentation Modes

*There are several ways a page of text can be analysed. The tesseract api provides several page segmentation modes if you want to run OCR on only a small region or in different orientations, etc.*

**Here's a list of the supported page segmentation modes by tesseract. Check it out here**

0    Orientation and script detection (OSD) only.  
1    Automatic page segmentation with OSD.  
2    Automatic page segmentation, but no OSD, or OCR.  
3    Fully automatic page segmentation, but no OSD. (Default)  
4    Assume a single column of text of variable sizes.  
5    Assume a single uniform block of vertically aligned text.  
6    Assume a single uniform block of text.  
7    Treat the image as a single text line.  
8    Treat the image as a single word.  
9    Treat the image as a single word in a circle.  
10    Treat the image as a single character.  
11    Sparse text. Find as much text as possible in no particular order.  
12    Sparse text with OSD.  
13    Raw line. Treat the image as a single text line, bypassing hacks that are Tesseract-specific.  

**To change your page segmentation mode, change the ```--psm``` argument in your custom config string to any of the above mentioned mode codes.**

### Playing around with the config

*By making minor changes in the config file you can* 
- specify language
- detect only digits
- whitelist characters
- blacklist characters
- work with multiple language

![image](https://github.com/Tanwar-12/OCR-in-Python-with-OpenCV-Tesseract-and-Pytesseract/assets/110081008/69b7f311-82b4-47a3-baf6-423336f04d35)

![image](https://github.com/Tanwar-12/OCR-in-Python-with-OpenCV-Tesseract-and-Pytesseract/assets/110081008/793687d6-178c-4558-83fe-d301d2321786)

![image](https://github.com/Tanwar-12/OCR-in-Python-with-OpenCV-Tesseract-and-Pytesseract/assets/110081008/df664595-2d68-4eed-99e5-2ce72adce45f)

![image](https://github.com/Tanwar-12/OCR-in-Python-with-OpenCV-Tesseract-and-Pytesseract/assets/110081008/9139966e-c12e-4476-9045-236c71fd8b30)

![image](https://github.com/Tanwar-12/OCR-in-Python-with-OpenCV-Tesseract-and-Pytesseract/assets/110081008/39c5a697-3bed-40df-a478-8fc6318c6c12)

![image](https://github.com/Tanwar-12/OCR-in-Python-with-OpenCV-Tesseract-and-Pytesseract/assets/110081008/7dbfecaa-a5b3-4553-8b06-045c89c6ea47)






