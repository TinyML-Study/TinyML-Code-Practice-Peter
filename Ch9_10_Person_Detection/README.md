
## Ch.9. Person Detection :running:


### Environment 

* [Arduino Nano 33 BLE](https://store.arduino.cc/usa/nano-33-ble-sense)
* [Arducam Mini-2MP-Plus](https://www.amazon.com/Arducam-Module-Megapixels-Arduino-Mega2560/dp/B012UXNDOY)


### Prerequisite :point_up:

1. Install 'JPEGDecoder' library via Arduino IDE library manager.
2. Download the [Arducam library](https://github.com/ArduCAM/Arduino) and copy the ArduCAM subdirectories into *Arduino/libraries*.
3. 


### Results :sparkles:

#### Person is not detected.:point_right: Red Light
<center>
<img src="../img/person_detection_3.jpeg" width="500">
</center>

#### Person is detected. :point_right: Green Light
<center>
<img src="../img/person_detection_4.jpeg" width="500">
</center>



###   The Basic Flow :surfer:

<center>
<img src="../img/person_detection_2.png" width="600">
</center>


#### Sequences
1. **`Image Provider`**'s **GetImage()** takes a picture from the camera. &rightarrow;
2.  **`tflite::MicroInterpreter`**' classifies the input and returns **output**. &rightarrow; 	
3. **`Detection Responder`** runs **RespondToDetection()** to order the response.





	  