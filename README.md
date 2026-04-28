An IoT-Based System for Comprehensive Patient Medication Monitoring
This project provides a simple, cost-effective IoT-based solution designed to help patients adhere to their daily medication schedule. It is particularly useful for elderly and chronically ill individuals who may forget or miss their doses. The system is built using the Arduino Uno and integrates components like DS3231 RTC, ultrasonic sensor, 16x2 I2C LCD, LED indicators, and a buzzer to deliver timely alerts and ensure accurate intake verification.

💡 Features
⏰ Time-Based Alerts: Uses a Real-Time Clock (RTC) to track medication times and activate reminders accordingly.
🔔 Visual and Audio Notification: Alerts patients with buzzer sound, LED indicator, and LCD messages when it’s time to take medication.
🤖 User Interaction Detection: Ultrasonic sensor detects when the box is opened, confirming user response.
🔁 Automatic Reset: Once the medication is taken, the system resets and waits for the next scheduled dose.
⚙️ Offline and Standalone: No Wi-Fi or remote monitoring needed; fully functional as an independent system.
🛠️ Hardware Requirements
Arduino Uno
DS3231 RTC Module
16x2 I2C LCD Display
Ultrasonic Sensor (HC-SR04)
LEDs (for slot indication)
Buzzer
Push Buttons (optional for manual override)
Jumper Wires and Breadboard
Power Supply
🧠 Software Implementation
Code written in Embedded C/C++ using the Arduino IDE
Real-time clock integration for scheduled checks
Event-driven logic to activate and reset alerts
Infinite loop structure for continuous monitoring
📚 How It Works
System checks the current time using RTC.
If it matches the stored medication schedule:
Activates LED, buzzer, and LCD alert.
Waits for the box to open (via ultrasonic sensor).
If box opened:
Deactivates alerts and resets for next dose.
📎 Conclusion
This project proves that even simple embedded systems can play a significant role in healthcare by improving medication adherence, minimizing supervision, and offering an accessible solution for daily medicine tracking.
