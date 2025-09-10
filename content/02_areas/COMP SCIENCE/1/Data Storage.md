
a bit is the basic unit of all computing memory storage terms and is either a 1 or 0
it comes from '**b**inary dig**it**'

a byte is the smallest unit of memory in a computer
1 byte is 8 bits

[[02_areas/COMP SCIENCE/1/Image Representation|Image Representation]]
[[02_areas/COMP SCIENCE/1/Sound Representation|Sound Representation]]
sound file calculation



---

Recall
b = bits
nibble = 4b
B = bytes = 8b
Kb = kilobit
Kib = kebibit
KB = kilobyte
KiB = kibibyte
Mb = megabit
Mib = mebibit
MB = megabyte
MiB = mebibyte


## task 1
You would need to divide the answer in bytes by 1024 3 times to get the answer in Gibibytes

There would be 1000x1500=1,500,000 pixels in an image that has a resolution of 1000x1500


## task 2
1
1920x1536x16=47,185,920 b
47185920/8=5,898,240 B
5898240/1024=5,760 KiB
5760/1024=5.625 MiB

2
1024x1536x24=37,748,736 b
37748736/8=4,718,592 B
4718592/1024=4,608 KiB
4608/1024=4.5 MiB
4.5/1024=0.00439 Gib
16/0.00439=3,644.647 photos

You can store 3644 photos on a 16GiB memory card.


3
44.1kHz = 44100Hz = 44100 bits per second
44100x8=352,800 bits per sample per second
352800x2=705,600 two channels

a) the size of a one second sample is 705600b

30x705600=21,168,000 b
21168000/8=2,646,000 B
2646000/1024=2,583.984 KiB
2583.984/1024=2.523 MiB

b)the size of a 30-second audio recording is 2.523 MiB


4
3x60=180 seconds
180+30=210 seconds
44100x210x16=148,176,000 b
148176000/8=18,522,000 B
18522000/1024=18,087.891 KiB
18087.891/1024=17.664 MiB
740/17.664=41.893 

You can typically store 41 songs on a 740MiB CD.


## task 3
44.1 kHz = 44100Hz
44100x16x10x60=423,360,000 b
423360000/8=52,920,000 B
52920000/1024=51,679.688 KiB
51679.688/1024=50.468 MiB

52920000/1000=52,920 KB
52920/1000=52.92 MB


50.468 Mebibytes or 52.92 Megabytes



## plenary
The number of bits used to represent a sound sample is known as the sampling resolution

15a
4096x2048x16=134,217,728 b
134217728/8=16,777,216 B
16777216/1024=16,384 KiB
16384/1024=16 MiB
the file size of an image taken by this camera is 16 Mebibytes.


review learning
www: remembered formulas for calculating file sizes
ebi: find out why sound is usually recorded in 44.1kHz
