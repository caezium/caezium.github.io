**bitmap: individual bits and pixels (tiny dots) to represent an image**



bitmap image file formats include
- BMP
- JPG
- GIF
- PNG
- TIFF

**Monochrome images**
1 bit for each pixel
0 being white, 1 being black

![[02_areas/COMP SCIENCE/1/attachments/Pasted image 20250321115059.png]]

![[02_areas/COMP SCIENCE/1/attachments/Pasted image 20250321115113.png]]
![[02_areas/COMP SCIENCE/1/attachments/Pasted image 20250321115131.png]]

8 bits =1 byte 256
16 bit =2 bytes = 65,536
24 bits= 16,777,216

*resolution* is width and height of the image, so **how many pixels there are**
the *color depth* is the **number of bits used to represent each color**, more colors, the better and greater the number of colors can be represented.


**file size = color depth x resolution**



---
## task 1
higher resolution = more pixels = more details = higher quality
higher resolution = more pixels = more data = larger file size

![[02_areas/COMP SCIENCE/1/attachments/Pasted image 20250321115605.png]]

bmp files are not compressed and of the highest quality
png files are compressed, but they use lossless compression, keeping quality while reducing file size
jpeg files are compressed, use even less file size, but loses quality


## task 2
\#fff white = 1111 1111 1111
\#000 black = 0000 0000 0000
\#ff0000 red = 11111111 00000000 00000000
\#0000ff blue = 00000000 00000000 11111111


## task 3
8x50x50=20,000 bits
4x100x100=40,000 bits

10000000x24=240,000,000 bits 
240000000/8=30,000,000 bytes
30000000/1024=29,296.875 kebibytes
29296.875/1024=28.61 mebibytes


## plenary
worksheet

review learning
www understood image representation
ebi remember how to calculate file size
