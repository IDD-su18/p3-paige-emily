# P3: first prototypes
## List of Questions
1. What features will work best in classifying our sensor readings?
2. How accurately will transmission rates reflect the degree of fracture?
3. How can we scan for fractures on bones with small surface areas (wrist, cervical spine, foot) without detecting too much noise (due to the closeness of the mic to the sensor)? 
4. What is the best method for sensing and actuating the bone? How do we collect that data (bluetooth, phone aux jack, microSD)?
5. How can we design our device's hardware such that we...
   - reduce the amount of pain the patient feels,
   - make the process intuitive,
   - and minimize the likelihood of human error? 

## Look and Feel Prototype
We imagine the full interaction for our prototype to go as follows:
1. Doctor opens the device's app, and plugs the sensor into the headphone jack
2. Doctor positions the sensor and actuator on opposite ends of the suspected fracture point
3. Doctor presses a button on the actuator, which sends a sound through the bone. The sensor will record this, and the GUI will update accordingly
4. (optional) Doctor can save these results to the patient's log, to be used for monitoring. The log will track the patient's healing over time.

### Graphical User Interface
After our contextual inquiry, doctors expressed interest in the GUI providing information about:
- the detected transmission rate
- the expected transmission rates for a healthy bone
- a graphical representation of the healing over time
- an interpretation of the reading (fractured or not fractured)
- what type of fracture was detected

Our GUI will have two functions: scanning and monitoring. The scanning portion will include information for each individual scan, with an option to save the reading to a patient's record. For now, we'll just include options for e-mailing the data, but in the future, this could be done using an [epic upload code](https://www.imedicalapps.com/2017/03/epic-haiku-upload-medical-documents-patients-chart/).

![alt text](/images/gui.png)

### Physical enclosures
Doctors expressed the need for the device to be portable, easy to move precisely, and to work without causing too much pain. Inspired by the design of [ultrasound probes](http://www.tenacore.com/service/ultrasound-tee-probe/), we plan on fitting the transducer in a pen-shaped enclosure, since this makes it easier to position precisely. We hope to design our sensor so that it can fit within any existing stethoscope, so that it is low cost. For testing, we will be using a [3d printed stethoscope head by GliaX](https://github.com/GliaX/Stethoscope).

![alt text](/images/physical_enclosure.png)

## Implementation Prototype
We have been testing with both a 3d printed bone and pig femur. We'll be getting additional bones soon, so we can begin to compare scans between a fractured and non-fractured bone. 
![3d printed bone](/images/3d_printed_bone.jpg)
![Pig femur in gel recipe](/images/pig_femur.jpg)
![Implementation prototype](/images/implementation_prototype.jpg)

Implementation Video: https://youtu.be/0C5WVhAsVF4

## Reflection
During this assignment, we learned that OpenSCAD files are tough to work with, pre-soldered wires never last, and carrying a pig femur around daily is not fun.  

## Presentation 
https://docs.google.com/presentation/d/1myo9QGSspp70GDENwiBE1i4PZWlbu830GBA4aXYuocU/edit?usp=sharing