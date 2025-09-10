sound must also be converted into a digital form in order to be stored, and processed by a computer

#### Analogue to Digital Convertor **ADC**
is used to convert **inputs to** digital signals

#### Digital to Audio Convertor **DAC**
convert digital signals **to outputs**



##### Analogue
analogue sound signals are continuous, lime what you hear

##### Digital
digital signals are discrete

![[02_areas/COMP SCIENCE/1/attachments/Pasted image 20250320085114.png]]

sound is digitized by repeatedly measuring and recording the sound wave



![[02_areas/COMP SCIENCE/1/attachments/Pasted image 20250320085132.png]]


#### Sample Rate
the number of samples taken in a second
measured in **hertz**

*1 hertz = 1 sample per second*

#### Sample Resolution
number of bits that are used to represent each sample
the larger the sample, the more accurate/amount of data there will be
a common sample resolution is 16-bit


---
**File size (bits) = sample rate x resolution x duration**

---

recall
you can represent characters in binary too. the main character sets to represent them in binary are Unicode and ASCII. 



## task 1
ADC is analogue to digital conversion. a computer takes in analogue sound input and converts it into digital signals, which it does by taking samples of recorded analogue sound at intervals known as the sample rate, it does not record the analogue sound one to one, therefore it is discrete. the sample resolution of the digital signal determines how much detail and variation the sound samples, like amplitude, can be. The higher the sample rate, the more the accuracy of the sound.
DAC is digital to analogue conversion, a computer plays/outputs its sound file in digital signals to analogue output devices to let the user hear what it has stored in the sound file. The computer can recognize the digital sound files because it was converted using ADC in a way so that it understands.


## task 2

![[02_areas/COMP SCIENCE/1/attachments/Pasted image 20250320091047.png]]
## task 3
resolution: 16 bits
sample rate: 44.1kHz
length: 3 minutes 30 seconds

length = 3x60+30=210 
44.1kHz = 44100 Hz

file size = 210x44100x16=148,176,000 bits
148176000/8=18,522,000 bytes
18522000/1024=18,087.891 kebibytes
18087.891/1024=17.664 mebibytes



## plenary
worksheet
![[02_areas/COMP SCIENCE/1/attachments/Pasted image 20250320091603.png]]
![[02_areas/COMP SCIENCE/1/attachments/Pasted image 20250320091617.png]]



review learning
www: understood the difference of the sound graphs for analogue and digital sound data
ebi: remember how to calculate file size and the units involved