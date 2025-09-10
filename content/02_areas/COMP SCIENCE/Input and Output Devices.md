```toc
```

### Key definitions

1. Barcode
    
    1. Properties[3], error checking
    2. Process of reading
    3. Application, benefits[3]
2. QR Code
    
    1. definition[3]
    2. advantages[4]
    3. disadvantages[2]
    4. applications
3. difference between B and Q[3]
    
4. Digital Cameras
    
    1. definition CCD[3]
    2. Quality of image[3]
    3. preview…[3]
5. Keyboard/keypad
    
    1. def[2]
    2. how - press, complete circuit, interrupt, calculate, refer
6. Optical Mouse
    
    1. pointing device
    2. LED
    3. CMOS uses[2]
    4. DSP get location
    5. Advantages[2]
7. Microphones
    
8. 2D scanner
    
    1. scan head
    2. function
9. 3D scanner
    
10. Touch Screens
    
    1. 3 types
    2. advantages of each
11. Actuators
    
    1. function
12. Light projectors
    
    1. DLP
        1. DMD chip - determine the resolution, consists a large number of micromirrors
    2. color wheel
    3. projection lens
    4. white light source
    

    
    **重要**
    

# Input Devices

> _“Try to remember what each device does, why it does it, and when it may be used” — Ms. Shala, 2024_

## Barcode scanners(readers)

### Barcode

- Series of **dark** and **light** horizontal parallel lines of varying thickness
    - in 1D
- This type of code includes a **check digit** for **validation**
- stores **30 digits maximum**

**Pattern**

- 3 guard bars - left middle and right
    
- Each digit is presented by bars of 1 to 4 blocks thick
    
- Each digit is made up of 2 dark lines and white lines
    
- A barcode should be scanned when **aligned horizontally**
    
    ![Untitled|594x842](https://prod-files-secure.s3.us-west-2.amazonaws.com/81302f27-4907-4655-bf16-b52b2ac29be7/990843ba-b75d-454b-a7b8-9e41e7b17215/Untitled.png)
    
    - Left side - an odd number of dark elements; begins with a light bar
    - Right side - an even number of dark elements; begins with a black bar

### Process of reading

1. A barcode reader shines a **red laser**
    - by red **LED**
2. light is reflected back off the barcode
    - dark area - little or no light reflected back
    - allows the bars to be read
3. The reflected light is red by sensors
    - **photoelectric cells**
4. The different levels of reflection are converted into digital form as binary data
    - allows microprocessor to process the barcode


### Application

- Barcodes are most commonly found at the **checkout** in supermarkets
    
    - The scanned barcode number can be act as the key field in stock item record in the stock database
    - 不是非常清楚是否要考在此处运用的好处

- Tracking a package through the delivery process
    
- Register borrowed books in libraries
    

### Advantages

- **Efficiency**
    - Faster input informations into a system compared to typing
- **Accuracy**
    - Less human error by manually data entry
- **Traceability**
    - automated stock control
    - more easier tracking of information

### Disadvantages

1. hard to guard against damage
    - almost no redundant data(duplicated)

## QR codes - Use Cameras

### Quick Response Code

- code made up of a **matrix** of filled-in dark squares on a light background
- in 2 Dimension
- Can hold up to **7089 digits**
    - usually an **internet address** is encoded within the QR code
- **Three large square** in the corners is used as **alignment**
    - used to ensure a **correct size and orientation** of a barcode that can be scanned from any direction

### Advantages

- It can hold much **more information**
- will be fewer errors
    - have builtin **error-checking** systems
- Easier to be scanned
    - do not need a **laser** or **LED scanner**
    - They can be scanned by **cameras**
- easy to **transmit** QR codes to transfer
- Greater **informational security**
    - can encrypt QR codes

### Disadvantages

1. have more than one QR code format
2. can be used to transmit malicious codes
    - ‘attagging’
    - could gain access to everything on a device
    - could led a user to sent to a fake website

### Applications

1. Advertisement for products
    - frame QR codes
        - Have advertising logos in ‘canvas area’
        - not usually free
2. giving automatic access to a website or contact number
3. store boarding passes or VISA electronically

### How does it functions

1. Point the phone or tablet camera at the QR code
2. App will process the image taken by the camera and convert squares into readable binary data
3. data will be read differently based on their formats
    1. If it is a web address → send to browser software
    2. a telephone number → send to telephone app
    3. boarding pass → send to or download to the phone.

## Differences between QR code & Barcode

1. Barcode is 1D and QR code is 2D
2. barcode use vertical lines and QR codes use squares
3. QR code hold more data than a barcode
4. QR code can be read from any angle and barcode usually should be lined up
    - QR is faster to be scanned
5. barcodes are used in checkouts and QR codes are used in various field such as advertisement

## Digital Cameras

- It works by capturing light and converting it into a digital image
- It link to a computer system via a USB port or by using wireless Bluetooth

### How does it works

1. First, an aperture opens at front of the camera to allow light enter
2. Light passes through lens onto a **light-sensitive cell**(CCD)
    - This cell is made up of millions of **tiny sensors** acting as photodiodes
        - Each of these tiny sensors are referred as pixels
    - CCD → convert **light** into **electricity**
3. Then, the image is converted into tiny electric charges and are then passed through an **ADC** to form a **digital image array**
    - **levels of brightness**
        - e.g. a 8-bit ADC would have 2^8 possible brightness levels per pixel
    - **measure of color**
        - usually use 8-bits for each primary color

---

- The quality of image is depends on
    - the quality of lens & sensor array
    - number of pixel used
    - levels of light
    - format of image

### Advantages

- digital cameras allows preview of image
- The image created can be easily duplicated and transmitted via network connection
- have software that support editing facilities

### Applications

- integrated into phones
- security systems
- professional photographers

## Keyboards/Keypad

- most common method used for **text-based data entry**
    - connected to the computer by **wire** or **wireless** connection
    - It is **relatively slow** and **prone to errors** but still the **easiest way** to enter text
- For laptops - physically builtin
- For phones - It can be **virtual** that requires a type of touch screen technology

### How does it functions

1. **Membrane** and circuit board present at base of keys
2. when a key is pressed, it **complete a circuit**
3. It also generate a hardware interrupt
    - added to a buffer to be wait to be processed
4. the CPU can **calculate the location** of the keypress
    - Each character on a keyboard has a corresponding **ASCII value**
    - CPU refer to an **index file** to identify which character the keypress represents

### Other knowledges

- Ergonomic keyboards - designed to prevent injuries

## Optical mouse

- It is a **pointing device**
- have tiny cameras to take **1500** images per second
- It can work on any surface

### How does it works

1. **Red LED** is shined from the bottom onto a surface
2. **Reflection** of the light can be pick up by a **CMOS**
    - **complementary metal oxide semiconductor(CMOS)**
        - used to detect the mouse movement
        - take tiny images of surface continuously
        - generate electric pulses to represent the reflected red light (image)
3. Generated pulses are sent to DSP
    - **Digital signal processor(DSP)**
        - can work out the **coordinates** of the mouse based on the **changing image patterns** when moving
        - can determine the velocity
4. The computer can move the **on-screen cursor** to the coordinates sent by the mouse

### Advantages

- There are no moving part, more reliable
- dirt can’t get trapped in any of the mechanical components
- no need to have any special surfaces

### Wired vs Wireless

- **Bluetooth connectivity**
    - more **versatile**
- **USB wired connection**
    - **no signal loss** due to constant wire connection
    - **cheaper to operate**
        - no need to charge batteries
    - no need to **change old batteries**, less environmental impact

## Microphones

- Device that is used to **convert** **sound waves** into **electrical signals** that can be processed by the computer
    - **capture** and **convert** analogue sound into digital sound
- can be **built** into computer or be **external** devices
### How does it functions

1. Sound cause the air to vibrate
2. A diaphragm picks up the vibration, the diaphragm also begins to vibrate
3. A copper coil is wrapped around a cone and is attached to the diaphragm
    - when diaphragm vibrates, the cone moves in and out causing the copper coil to move backwards and forwards
4. Motion cause the coil to send **electric current**
    1. by the motion of cone to cut through the magnetic field around the permanent magnet
    2. This current is **analogue** in nature
5. The current is sent to a **sound card** to converts the current into a **digital signal**
    - sound card includes a ADC, DAC and other sound related devices
    - or the electric current can be amplified

## 2D scanners

- used to input hard copy documents into digital forms

### How does it functions

1. document is placed on a glass panel
    1. close the cover to prevent light invervention
2. scanner shines a light onto the surface of a document to illuminate it
    - use LED or xenon lamp to produce very bright white light
3. A **scan head** **move across** the document to reflect the light reflected from the page until the whole page has been scanned
4. The reflected image of document is sent to a lens using series of mirrors
    1. to focus the document image
5. The focused image falls onto a charge couple device(CCD), converts light into an electric current
6. Then, the image is passed through an **ADC** to form a **digital image**
    - can use OCR software to be converted into a text file format

### Application

1. airport to read passports
2. integrated with printer

## 3D scanners

- used to scan solid objects and produce a 3D image
- e.g. lasers, magnetic, resonance 3D printer

### How does it simply works

- A scanner shines a laser over serval points along the surface of a 3D object
- Record measurements of the geometry of the object
- measurements are converted to digital file and produce 3D model

### Application

- Computed tomographic (CT)

## Touch Screens

- It is a very **common form** of input device
- It allows simple touch selection operation
    - e.g. from a menu to launch an application
- It allows the user to carry out the same functions as pointing devices(e.g. mouse)
- There are three common types of touchscreen
- **Use of microcontroller**
    - A microcontroller converts the voltage (created when the two resistive layers touch) to digital data, which it then sends to the microprocessor.

### Resistive touch screens


- **Structure (not necessary)**
    
    - made up of **two layers** of electrically resistive material with a voltage applied across them (shown in second graph by two transparent **electrode**)
    - **Upper layer**
        - made of **flexible polyethylene**
        - have a **resistive coating** on one side
    - Bottom layer
        - made of **glass**
        - have a **resistive coating** on one side
    - In between
        - two layers are **separated** by air or inert gas
- **Process of detect**
    
    1. When the top polyethylene surface is touched, the two layers make contact.
    2. Both layers are coated in a resistive material a circuit is now **completed** which results in a **flow of electricity.**
    3. The point of contact is detected where there was a **change in voltage**.
- **Advantages**
    
    1. cheaper
    2. Can be used with bare fingers, stylus and gloved hand
    3. Good resistance to dust and water
- **Disadvantages**
    
    1. Low touch sensitivity (sometimes have to press down harder)
    2. Doesn’t support multi-touch facility
    3. Poor visibility in strong sunlight
    4. Vulnerable to scratches on the screen (made of polymer).

### Infrared touch screens

- Infrared touch screens use a glass screen with an array of **sensors** and **infrared transmitters**
    
    (e.g. above image)
    
- Infrared transmitters emit beams cover the screen in a matrix pattern
    
- Infrared sensors are placed around the edge of the screen to detect the infrared rays
    
- **Detect Process**

    1. If any of the infrared beams are broken, the radiation reaching the sensors is reduced
    2. The changed sensor readings are sent to a microcontroller that calculates where the screen was touched
- **Advantages**
    
    1. Better image quality
    2. Allows multi-touch facilities
    3. good screen durability
    4. the operability isn’t affected by a broken screen
- **Disadvantages**
    
    1. expensive
    2. Screen can be sensitive to water or moisture
    3. The infrared beams could be disturbed accidentally
    4. (Based on above reason) Sometimes sensitive to light interference

### Capacitive touch screens(most common)

- **Contains 3 layers**
    1. protective layer
        - a transparent layer of glass
    2. conductive layer
        - a transparent layer of electrode
    3. glass substrate
- **Method of detection**
    
    1. the **electrostatic field** of the conductive layer is changed when **bare fingers** touch the screen
    2. the installed **microcontroller** is able to calculate **where** this change took place
- **Two main types of capacitive touch screens**
    
    
    ### Surface Capacitive Screen
    
    
    - Sensors placed at the **corners(4 corner electrodes)**
    - **Electric fields** across the surface of the screen is created by the **supplied voltage** to each of the corners
    - When a finger or a stylus touches the screen, it reduces the capacitance and draws current from each corner
    - A microcontroller measures the decrease in **capacitance** to determine the **exact point** of contact
    
    ### Projective Capacitive Screen

    
    - the transparent conductive layer(electrode) arranged in an X-Y matrix pattern
        - **NOTE**: the colored region are still belongs to the conductive layer
    - It generates a **three-dimensional electrostatic field** over the surface of the screen by the electrode **oscillate** at a **known frequency**
    - **Any touch** _(from a bare finger, a stylus, or even thin gloves like surgical or cotton gloves)_ disturbs this **3D electrostatic field** and **reduce** the **capacitance**
    - The **disturbance** in the electrostatic field is detected by a **microcontroller**, which then calculates the **coordinates** of the touch point
    
    ||Surface Capacitive Screen|Projective Capacitive Screen|
    |---|---|---|
    |Device used|Sensors placed at the **corners(4 corner electrodes)**|the transparent conductive layer(electrode) arranged in an X-Y matrix pattern|
    |Theory|Electric fields across the surface of the screen is created by the supplied voltage to the corners|It generates a three-dimensional electrostatic field over the surface of the screen by the|
    |electrode oscillate at a known frequency|||
    |Interaction|When a bare finger or a stylus touches the screen, it reduces the capacitance at that specific location and draws current from each corner|Any touch, including those from a bare finger, a stylus, or even thin gloves like surgical or cotton gloves, disturbs this 3D electrostatic field|
    |Detection Method|A microcontroller measures the decrease in capacitance to determine the exact point of contact.|The disturbance in the electrostatic field is detected by a microcontroller, which then calculates the coordinates of the touch point|
    ||||
    
    ### Comparison
    
    ||Surface Capacitive Screen|Projective Capacitive Screen|
    |---|---|---|
    |Advantages|Cheap|1. More **durable** due to the conductive layers being protected by thick glass|
    
    1. capable of registering **multiple** simultaneous touches
    2. More sensitive to touches | | Disadvantages | Doesn’t support multi-touch | more expensive due to complex design |
- **Advantages**
    
    - Better image clarity than resistive screens, especially in strong sunlight
    - Very durable screens that have high scratch resistance, unlimited touch life
    - Allow multi-touch(**Projective capacitive screens**)
- **Disadvantages**
    
    - Surface capacitive screens only work with **bare fingers** or a special stylus
    - They are sensitive to electromagnetic radiation

# Output Devices

## Actuators

- It is a mechanical or electromechanical device that is used to **physically** **control the movement of devices**
    - eg.g open/close a valve

## Light projectors

- Projectors are used to project computer output onto **larger screens**

### Digital light projectors(DLP)

![Untitled|594x842](https://prod-files-secure.s3.us-west-2.amazonaws.com/81302f27-4907-4655-bf16-b52b2ac29be7/82a2d321-bd10-4083-9829-ae7715d8545d/Untitled.png)

- It use **DMD chip** to determines the **resolution** of the digital image
    - DMD - **digital micro-mirror device**
    - large number of micro mirrors in a matrix
    - each mirror creates a **pixel** in the image
- For each **micro mirrors**
    - ON - tilt towards the light source
    - OFF - tilt away from the light source
    - it can switch serval **thousands times** a second
        - which can help to create grey shades
    - **These mirror reflect lights towards projection lens**
- A bright white light source passes through a **color wheel** to **create color**
    - can create more than 16 million colors (256^3)
- It is used to project image on wall

### Liquid crystal display(LCD)

- **older technology** than DLP
- It use a high-intensity beam of light pass through **3 LCD screens** and onto a screen

![Untitled|594x842](https://prod-files-secure.s3.us-west-2.amazonaws.com/81302f27-4907-4655-bf16-b52b2ac29be7/aca11d58-19e9-48a5-ac1e-d55f187eef6c/Untitled.png)

**How does it functions**

1. Light source
    - beam of white light generated
2. Dichromic Mirrors
    - Light beams sent to a group of dichromic mirrors
    - reflect light back at **different wavelengths**
    - Thus, divide light into **red, green and blue** components and reflected **respectively**
3. Light components pass through **three LCD screens**
    - each LCD screens can either **block light** or **let it through**
    - each produce **monochromatic image**
4. Different versions of the same image are now produced
5. These images are recombined into a **single light source** using a special prism to produce a full color image
6. The image passes through the projector lens onto a screen

### Advantages & Disadvantages

![Untitled|594x842](https://prod-files-secure.s3.us-west-2.amazonaws.com/81302f27-4907-4655-bf16-b52b2ac29be7/8108dfbe-81c0-4c15-b0cf-a15f2ae0d350/Untitled.png)

## Printers - hard copies

![Untitled|594x842](https://prod-files-secure.s3.us-west-2.amazonaws.com/81302f27-4907-4655-bf16-b52b2ac29be7/07f75d79-ba6e-4213-86e2-398e9dad6861/Untitled.png)

- **3 color used for printing**
    - blue, yellow and magenta

### Inkjet printer

**Components**

- a moving print head
    - consists of **nozzles** that spray int onto paper
    - There are different **ink droplets technologies**
    - Liquid is dropped from **ink cartridge** through **fine nozzle** onto the pages
- ink cartridges
    - can be **one cartridge for each** three color + black
    - or **one single cartridge containing all** three color + black
- a stepper motor and belt
    - moves the print head across the page
- a paper feed
    - feeds the printer with pages

**Ink droplet technologies**

1. **Thermal bubble**
    - resistors create heat to makes ink to vaporize
    - cause ink to form tiny bubble
    - ink is ejected on paper when bubble collapse
        - It also create a small vacuum to draw fresh ink into the print head
2. **Piezoelectric**
    - A **crystal** is located at the back of ink reservoir for **each nozzle**
    - The crystal is given **a charge** to cause it **vibrate**
    - **vibration** force ink to be ejected onto paper

![Untitled|594x842](https://prod-files-secure.s3.us-west-2.amazonaws.com/81302f27-4907-4655-bf16-b52b2ac29be7/61b77f05-be11-427e-98c5-76f99b5784f8/Untitled.png)

### Laser printer

- It use dry powder ink
- It make use of properties of **static electricity** to produce text and images
- It utilize the **charge of toner** and **piece of paper**, heat is used to **bond** the particles to the paper

**Components**

1. **powdered toner cartridges**
2. **charged printing drum**
3. **fuser** - melt ink onto paper
4. **discharge lamp** - remove charge from the drum

![Untitled|594x842](https://prod-files-secure.s3.us-west-2.amazonaws.com/81302f27-4907-4655-bf16-b52b2ac29be7/2453eb73-8015-497d-918b-05878376f1d6/Untitled.png)

### Applications

- **Inkjet**
    - produce high quality, colored hard copies of **digital images**
    - It cost low and have smaller physical size
    - Prints relatively slow
- **Laser printer**
    - Produce high quality of printout **documents**
    - Can print very fast
        - good to make multiple copies of a document
    - **Advantages**
        - larger toner cartridges
        - larger paper trays
    - **Applications**
        - bulk print out of flyers in high volume
        - question paper

## 3D printer

![Untitled|594x842](https://prod-files-secure.s3.us-west-2.amazonaws.com/81302f27-4907-4655-bf16-b52b2ac29be7/61083290-60cc-468f-b883-3ca2224844ed/Untitled.png)

- **3D Printers:**
    - Devices used to produce solid objects with functionality.
    - They use **additive manufacturing** technology, primarily based on inkjet and laser printer technologies.
- **Additive Manufacturing:**
    - This process builds an object layer by layer from materials such as **powdered resin, metal, paper, or ceramic.**
- **Subtractive Manufacturing (Traditional Method):**
    - Involves the removal of material from a larger block to create an object, such as carving a statue from stone or machining parts from metal.
- **Types of 3D Printing:**
    - **Direct 3D Printing:**
        - Similar to conventional printing where a print head moves in multiple directions, layering materials directly to form an object.
    - **Binder 3D Printing:**
        - Involves two passes; the first pass applies dry powder and the second pass sprays a binder (glue) to form solid layers.
    - **Newer Techniques:**
        - Use lasers and UV light to harden liquid polymers, enhancing the variety of producible products.

**Applications**

1. Fashion and art
2. precision reconstructive surgery
3. make specified part of component that is not in mass production

## (Loud)Speakers

- Output devices that **produce sound**
- digital sound is changed into a electric current using digital to analogue converter(DAC)
- It is then pass through an amplifier to drive a loudspeaker
- The loudspeaker converts the current into a sound wave

![Untitled|594x842](https://prod-files-secure.s3.us-west-2.amazonaws.com/81302f27-4907-4655-bf16-b52b2ac29be7/2df1e8ca-2246-4221-8e4c-26d5b80cf2d4/Untitled.png)

## Monitors

![Untitled|594x842](https://prod-files-secure.s3.us-west-2.amazonaws.com/81302f27-4907-4655-bf16-b52b2ac29be7/05e4dca9-b279-49de-9d6e-288bffc3a8d6/Untitled.png)

### LED screens

- made up of tiny LEDS
- each LED is in either red, green or blue
- By varying the electric current sent to each LED, different color can be produced
    - by controlling colors
- OLED is an advanced version of LED
- **Application -** large outdoor displays

![Untitled|594x842](https://prod-files-secure.s3.us-west-2.amazonaws.com/81302f27-4907-4655-bf16-b52b2ac29be7/0babd632-fb91-4a65-850c-59075ddd12ab/Untitled.png)

> THERE IS A DIFFERENCE BETWEEN **LED SCREEN** AND **LED BACKLIT!**

### LCD screens

- made up of tiny liquid crystals
- The state of these crystals can be changed in applied electric field
    - **opaque** or **transparent** to allow light to pass
- It need a **backlit** to function
    - There are CCFL(**cold cathode fluorescent lamp)** and LED backlit

**CCFL vs LED**

- LED can reach **maximum brightness** immediately
- LED have more vivid colors
- LED can have better definition&contrast level
- LED can make screen more thin
- LED is more long lasting, thus reliable
- LED consume less energy

**Benefits**

- Low power consumption
- cooler running temperature
    - less heat
- do not suffer image burn
- brighter color
- higher resolution
- cheaper

### OLED screens

- It use organic materials to create semi-conductors
    - metallic cathode and glass anode
- when electric field is applied to the electrodes, they give off light
- no backlighting is required
    - can be very thin
    - can be **bend screens to any shape**

![Untitled|594x842](https://prod-files-secure.s3.us-west-2.amazonaws.com/81302f27-4907-4655-bf16-b52b2ac29be7/3cce02f0-b8e2-42a8-83dc-00013b7ef85b/Untitled.png)

**Advantages**

1. Thinner, lighter and more flexible than LEDs and LCDS
    - plastic, organic layers vs crystal structures
2. It gives a brighter light
3. Consume much less power
    - It do not require backlighting
4. Can be made into large size
5. have large field of view
    - 170 degrees

# Sensors

- definition
    - Sensors are **input devices**
    - Read **physical properties** from their surroundings