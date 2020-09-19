
## Ch.9. Person Detection :running:

<br>

##   The Basic Flow :surfer:

<center>
<img src="../img/person_detection_2.png" width="600">
</center>


#### Sequences
1. **`Image Provider`**'s **GetImage()** takes a picture from the camera. &rightarrow;
2.  **`tflite::MicroInterpreter`**' classifies the input and returns **output**. &rightarrow; 	
3. **`Detection Responder`** runs **RespondToDetection()** to order the response.





	  