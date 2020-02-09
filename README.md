# Garage48 Arts & Robots "BabyVanker" project
Robot triggering rocking of the baby stroller when crying is detected.
And also pretty cool tail/tentacle with many possible weird/fun applications.

* For rocking we've used Servo and artificial tail from silicon (aka soft robotics).
* Cry detection is implemented using pre-trained Tensorflow model from Tensorflow lite (https://github.com/tensorflow/tensorflow/tree/master/tensorflow/lite/micro/examples/micro_speech).
 Model recognizes "yes" and "no" keywords, and detects speech in general - "unknown". Baby cry sometimes get recognized as "yes" by model so I was able to reuse it.
 * We've used Arduino Nano BLE 33 Sense (https://www.arduino.cc/en/Guide/NANO33BLESense) - it has microphone, bluetooth and lots of other sensors.
 * To disable motion triggering (to avoid noizy distraction during presentations of peers during hackathon) we've used Magnet detection using Arduino_LSM9DS1 library. (We were too short on time to add On/Off switch) 
 * Proto-threading patter is used to deal with concurrency

P.S. LasteVanker means baby-stroller in Estonian
 
 
