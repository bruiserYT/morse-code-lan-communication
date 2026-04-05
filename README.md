# morse-code-lan-communication
Real-time Morse code communication system over LAN using Python sockets with timing-based encoding and decoding.


## Overview

This project implements a real-time Morse code communication system using Python socket programming over a Local Area Network (LAN). The system enables secure and lightweight message transmission by converting keyboard inputs into Morse code signals and decoding them at the receiver end using timing-based interpretation.

The implementation and testing of the system were carried out using Jupyter Notebook, making it easier to experiment with real-time input handling, timing analysis, and debugging.

---

## Features

* Real-time Morse code transmission over LAN
* Keyboard-based input using space key
* Timing-based decoding for dots, dashes, letters, and words
* Non-blocking socket implementation for continuous reception
* Developed and tested using Jupyter Notebook
* Low bandwidth communication
* Extendable to hardware and wireless systems

---

## Technologies Used

* Python 3
* Socket Programming (TCP)
* pynput library for keyboard input
* Jupyter Notebook for development and testing
* Time-based signal processing

---

## Project Structure

sender/        Morse code sender script
receiver/      Morse code receiver script
notebooks/     Jupyter Notebook implementation (optional)
docs/          Project report and diagrams
demo/          Demo recordings (optional)

---

## Installation

Clone the repository:

git clone https://github.com/your-username/morse-code-lan-communication.git
cd morse-code-lan-communication

Install dependencies:

pip install -r requirements.txt

(Optional) Install Jupyter Notebook:

pip install notebook

---

## Usage

Step 1: Start Receiver

cd receiver
python receiver.py

Step 2: Start Sender

cd sender
python sender.py

Alternatively, the system can be executed and tested within Jupyter Notebook for interactive experimentation.

Ensure that the receiver IP address is correctly set in the sender script before execution.

---

## Controls

Press SPACE quickly to generate a dot
Hold SPACE longer to generate a dash
Pause approximately one second between letters
Pause approximately two seconds between words
Press ESC to exit the sender

---

## Working Principle

The system detects the duration of key presses to classify input as either a dot or a dash. Each signal is transmitted instantly over a TCP connection. The receiver collects incoming signals and uses timing gaps to determine character and word boundaries. A predefined Morse dictionary is used to decode the signals into alphabetic text.

Jupyter Notebook was used during development to test timing thresholds, debug socket communication, and validate decoding logic interactively.

---

## Applications

Secure communication in defense systems
Emergency signaling systems
Low-bandwidth communication environments
Educational demonstration of communication concepts

---

## Future Scope

Integration with hardware push-button devices and microcontrollers
Implementation over wireless communication systems such as RF or LoRa
Addition of encryption for enhanced security
Development of mobile or embedded system versions

---

## License

This project is open-source and available under the MIT License.

---

## Author

YASH THAKRE
Electronics and Computer Science
Mumbai, India
