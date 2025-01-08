# 🚀 Electronic Fare Collection System Automation 🚀

This project is designed to develop a cost-effective and user-friendly Electronic Fare Collection System (EFCS) suitable for small-scale public transportation systems. 
The system utilizes IoT technologies to provide digital payment and vehicle tracking.

## 🌟Project Summary
The Electronic Fare Collection System (EFCS) is developed by integrating a Raspberry Pi, NFC card reader, and GPS module. The system collects fares by scanning passenger cards, 
tracks vehicle locations, and transmits this information to a central database.

### 🛠 Features
- *IoT-Based Solution:* Data collection with NFC card readers and GPS module.
- *Raspberry Pi Infrastructure:* Economical and flexible hardware solution.
- *Python Software:* Algorithms for payment and location tracking.
- *User-Friendly Interface:* Card balance inquiry and top-up.
- *Future-Compatible:* Infrastructure ready for QR code and mobile NFC integration.

## 🔧 Hardware Used
- *Raspberry Pi 4B (4GB)*
- *PN532 NFC Card Reader*
- *NEO-6M GPS Module*
- *7-inch Touch Screen*

## System Architecture
The system consists of three main components:
1. *Bus Devic:* Operates with NFC readers and a GPS module.
2. *User Interface:* Processes card balance inquiries and top-ups.
3. *Corporate Management Panel:* Manages payments, locations, and financial transactions.

## Project Setup
### 1. nstallation of Required Software
- Raspberry Pi operating system: [Raspberry Pi OS](https://www.raspberrypi.com/software/)
- PPython libraries: pandas, flask, mysql-connector, pyserial
- Database: *MySQL*

### 2. Hardware Connections
1. *NFC Module:* Connected to the Raspberry Pi GPIO pins.
2. *GPS Module:* Connected via UART.
3. *Touch Screen:* Connected using the Raspberry Pi's DSI port.
   
## 🎮 Usage

### 1. Bus Device
- *When a card is scanned:* Checks balance, if sufficient, payment is deducted.
- *Location tracking:* GPS data is sent to the central system every 2 seconds.

### 2. User Interface
- *Balance Inquiry* Users can view their balance using their national ID number.
- *Balance Top-Up: * Users can add funds to their cards online.

### 3. Management Panel
- *Personnel and card management.*
- *Tracking vehicle locations.*
- *Revenue and transaction reports.*

## Test ve Değerlendirme
- *Functional Tests:* Accuracy of payment and balance transactions tested.
- *Security Tests:* User information protected with data encryption.
- *Field Tests:* System performance evaluated in real buses.


## 📞 Contact


- 📧 elfaltntas123@gmail.com  <br/>
You can find detailed information about the project at the link below:

[BUS AUTOMATION PDF Dökümanı](https://github.com/elfaltntas/EUTS-BUS-AUTOMATION/blob/main/BUS%20AUTOMATION.pdf)
