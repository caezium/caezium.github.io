Compression is the process of **reducing** the size of a file by encoding the **data in a way that it uses less bits, less space.**
Minimize the amount of space needed or bandwidth required for transmission, while still allowing the original data to be reconstructed when needed.

Compression can be:
- **lossless**
	- **no data is lost**
- **lossy**
	- **some data is discarded to reduce size**


### Run-Length Encoding (RLE)
simple form of lossless compression for files that have sequences of **repeated characters or data.**

It encodes consecutive repeated elements (runs) as a single data value with a count of how many times that value is repeated.
ex. images with large areas of uniform color

Original Data `AAAAABBBCCCCDD`
RLE Encoding `5A3B4C2D`

if ASCII
`aaaaabbbbccddddd`
`05 97 04 98 02 99 05 100`

![[02_areas/COMP SCIENCE/1/attachments/image.png]]


### Impacts of Compression
- less **bandwidth** requires
	- less data so less data needed for transmit.
- less **storage space**
- shorter **transmission time**

---

Recall

resolution of an image is the number off pixels used
color depth of an image is the number of bits used to represent color values of a pixel
hertz is samples per second

## green task

compression can help them save costs. cloud storage requires money, the less data you store, the more you save, so by compressing their files, they can save costs.

```
The file size of the compressed file will be smaller (1) so take up less storage space (1) or be faster to upload / transmit / email (1).
```
## amber task

G5R3y6R3G4

```
G5R3Y6R3G4 – usually the amount comes first e.g. 5G3R6Y3R4G
```
## red task

reducing the resolution of an image will make it have less pixels, make it seem blurry or not correct. Reducing the color depth of an image will not allow some colors to be correctly represented, making the image not accurate.

```
Reducing the colour depth or resolution will result in a reduced file size. (1)  
Data will be permanently lost by doing this. (1)  
A reduction in colour depth will give a reduced number of colours that can be used resulting in a lower quality image / gradations will have sudden changes in colour. (1)  
A reduction in the resolution / number of pixels in the image will result in the image being lower quality (assuming both images are displayed at the same physical size). (1)  
Accept other appropriate examples of how resolution and colour depth changes affect image size.
```

## plenary

it is a form of lossless file compression. it reduces sizes of repeated data.

3W2D5W4D3W1D1W2D1W1D1W16D1W1D1W2D1W1D3W4D5W2D3W

46 characters -> 46 bytes

8x8 grid uses -> 64 bytes

saved = 64-46 = 18 bytes

-1 byte saved because need a byte to state that it is using RLE

```
21 a -

It is a form of lossless file compression: 

• It reduces the size of a string of adjacent, identical data. 

• A repeated string is encoded into two values: 

• The first value represents the number of identical data items. 

• The second value represents the code of the data item. 

• RLE is only effective where there is a long run of repeated units.

B i

3W 2D 5W 4D 3W 1D 1W 2D 1W 1D 1W 16D 1W 1D 1W 2D 1W 1D 3W 4D 5W 2D 3W

ii 

8 × 8 grid requires 64 bytes of storage 46 bytes (47 bytes) are used in the RLE code reduction = 64 − 46 = 18 bytes (17 bytes)
```

review learning
www understood what compression does and its advantages
ebi remember RLE and file saving calculations

---
#### lossy and lossless extended
*lossy*: loses detail **permanently**
*lossless*: does not lose detail, reversible


**Lossless** is important for files where any loss of data would be disastrous. eg large spreadsheet, or a large computer application


**Lossy file** compression eliminates unnecessary data from the file.
This means that the original file cannot be reconstructed once it has been compressed.
![[02_areas/COMP SCIENCE/1/attachments/Pasted image 20250403091306.png]]

it can be applied to 
- an image: reduce resolution and/or color depth
- sound file: reduce sampling rate and/or resolution

##### Common lossy file compression algorithms are
- *MPEG-3 (MP3)*
	- **sound files**
	- retain an acceptable quality of the sound
	- reduce by about 90%
	- **removal of sounds outside human ear range**
	- if two sounds are played at the same time, it will keep the louder one as the ear can only hear the louder one: perceptual music shaping
- *MPEG-4 (MP4)*
	- **multimedia files** - music, videos, photos
	- **retain an acceptable quality** of the sound and video
- *JPEG*
	- used for **bitmap images**
	- human eyes don't detect differences in color shades quite as well as brightness
	- separating pixel color from brightness, images split into 8x8 pixel blocks, then allows certain information to be discarded without causing any real noticeable deterioration in quality.



---

Recall

software refers to a collection of programs, data, and instructions designed to perform a specific task and provides functionality for the user.

hardware refers to a collection of physical components that are required for a computer system to function.

## green task

a music track should use lossy compression most of the time because you can remove ranges that the human ear can't hear. You should use lossless compression to preserve audio quality.

a text document should use lossless compression to not lose text

a video clip should use lossless compression to make sure it keep quality

a web image should use lossy compression to make loading times faster

a software application should use lossless compression so it still works and doesn't lose its instructions

a database should use lossless compressions so it doesn't lose data.




model

|                        |                  |                                                                                                                                                                                     |
| ---------------------- | ---------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Use                    | Lossy / Lossless | Reason                                                                                                                                                                              |
| A music track          | Lossy            | Some recorded sounds are not detectable by the human ear, and no noticeable difference will be heard if some sound data is lost. (Some music purists may prefer a lossless format.) |
| A text document        | Lossless         | All characters in a text document must be preserved.                                                                                                                                |
| A video clip           | Lossy            | Video data can easily be lost without affecting the quality too much.                                                                                                               |
| A web image            | Lossy            | Images can still be recognised easily, even with the type of loss that the format uses.                                                                                             |
| A software application | Lossless         | A software program may not run if a single character of data is missing.                                                                                                            |
| A database             | Lossless         | Data must be reproduced exactly.                                                                                                                                                    |

## amber task

I might compress photographic files before emailing them to upload it faster.

use less storage space so that it can be sent or received easier.

A draft manuscript for a book should use lossless compression when transmitting so that it doesn't lose any data or detail of the stuff in the book.

```
Reason 1. Files take less time for the receiver to download.

Reason 2: The file size may exceed the limit of what can be attached to an email.

Or another reason such as reducing the storage size on a friend’s computer / email storage quota.

(i) a draft manuscript for a book.

Lossless – the manuscript cannot lose any of its content while being transmitted.

(ii) A video recording which you have made of the school play.

Lossy – the file will be much smaller, and the quality will still be acceptable.
```
## red task

A video recording which you have made of the school play should use lossless compression as if you don't, the sending times and file size will be very very big.

```
Lossy – the file will be much smaller, and the quality will still be acceptable. Must be included within the bound of answers and should include why for the scenario. Easily portable, USB flash memory drive, email attachment etc.
```

## plenary

B

sample resolution

sound files, lossy compression

RAW files Raw bitmap files BMP

Run Length Encoding

```
A B AX1S

B Sampling/Sample resolution

C Lossy file compression

D Raw bitmap files (BMP)

E Run-length encoding (RLE)
```


Review learning

www understood key points of lossless and lossy compression

ebi understand more real life examples of when to use lossless and when to use lossy

Extra Activities

Summarize learning

worksheet