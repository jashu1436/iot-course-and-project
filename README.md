Motion Detection System using Arduino (IoT)








📌 Overview

This project presents a Motion Detection System using Arduino Uno and sensors to detect movement and provide instant alerts. It is designed as a low-cost, efficient, and beginner-friendly IoT solution for security and automation.

🎯 Objectives

✔ Detect motion using sensors
✔ Provide alerts using LED & buzzer
✔ Reduce manual monitoring
✔ Build a cost-effective system
✔ Enable future IoT integration

🧠 Problem Statement

Conventional monitoring systems require continuous human supervision and can be expensive. This project solves that by providing an automated motion detection system with real-time response.

🛠️ Hardware Components
Component	Quantity
Arduino Uno	1
PIR Sensor / HC-SR04	1
LEDs (Red, Green)	2
Buzzer	1
Breadboard	1
Jumper Wires	Several
🔄 System Working

👉 The same workflow is shown in your project flowchart (page 9).

⚙️ Algorithm
Start system
Initialize Arduino pins
Read sensor input
Check for motion
If detected → Activate LED & buzzer
Else → Keep outputs OFF
Repeat continuously
💻 Code Snippet
int sensorPin = 2;
int ledPin = 3;
int buzzer = 4;

void setup() {
  pinMode(sensorPin, INPUT);
  pinMode(ledPin, OUTPUT);
  pinMode(buzzer, OUTPUT);
}

void loop() {
  int motion = digitalRead(sensorPin);

  if (motion == HIGH) {
    digitalWrite(ledPin, HIGH);
    digitalWrite(buzzer, HIGH);
  } else {
    digitalWrite(ledPin, LOW);
    digitalWrite(buzzer, LOW);
  }
}

👉 Full code available in your report (page 11).

📥 Input
Sensor detects motion or object presence
Ultrasonic sensor calculates distance using sound waves
📤 Output
🔴 Red LED → Object detected
🟢 Green LED → No object
🔊 Buzzer → Alert signal
✅ Results
Real-time motion detection
Instant alert system
Low power consumption
Accurate detection for small-scale applications
🚀 Future Enhancements

✨ Mobile notifications via IoT
✨ Cloud data monitoring
✨ Smart parking system
✨ Multi-sensor integration
✨ Automatic gate control

📚 References
Arduino Official Website
HC-SR04 Datasheet
Electronics Tutorials
IEEE Papers
👨‍💻 Authors
MD. Sahil Khan
T. Jaswanth
⭐ Acknowledgment

Special thanks to Ms. Baalne Anjali for guidance and support.

📌 How to Use
Connect components as per circuit
Upload Arduino code
Power the board
Monitor LED/Buzzer response

