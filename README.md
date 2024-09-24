# Advanced Keylogger

## Overview

The Advanced Keylogger is a Python-based application designed to capture and log keystrokes, screenshots, and audio recordings, providing comprehensive monitoring of user activity. It includes stealth mode, startup persistence, and secure data storage to ensure covert operation and maintain data integrity.

## Features

- **Keystroke Logging:** Captures and logs all keystrokes, allowing for detailed monitoring of user input.
- **Screenshot Capture:** Periodically takes screenshots of the user’s screen to visually document activity.
- **Audio Recording:** Records ambient audio through the microphone, providing an additional layer of information.
- **Stealth Mode:** Operates in the background without alerting the user, ensuring that the keylogger remains undetected.
- **Startup Persistence:** Configures the application to start automatically with the operating system, maintaining continuous monitoring.
- **Secure Data Storage:** Encrypts logged data using the Fernet encryption method to protect the information from unauthorized access.
- **Email Reporting:** Automatically sends the captured data to a specified email address for remote monitoring and analysis.

## How It Works

1. **Keystroke Logging:**
   - The keylogger captures keystrokes using the `pynput` library, logging them to a local file.

2. **Screenshot Capture:**
   - Screenshots are taken at regular intervals using the `Pillow` library and saved locally for review.

3. **Audio Recording:**
   - The application records audio using the `sounddevice` library, saving the recordings in `.wav` format.

4. **Clipboard Monitoring:**
   - Clipboard data is captured using the `win32clipboard` module, allowing for the monitoring of copied text.

5. **Data Encryption:**
   - Logged data, including keystrokes, system information, and clipboard contents, is encrypted using the `cryptography` library before being sent via email.

6. **Email Reporting:**
   - The keylogger sends the captured and encrypted data to a predefined email address, using the `smtplib` library to handle email communication.

## Technologies Used

- **Python:** Core programming language for developing the keylogger.
- **pynput:** For capturing keyboard input.
- **Pillow:** For taking screenshots.
- **sounddevice:** For recording audio.
- **cryptography:** For encrypting logged data.
- **smtplib:** For sending emails with the captured data.
- **pywin32:** For accessing Windows clipboard data.
- **scipy:** For handling audio file formats.

## Legal Disclaimer

This keylogger is intended for educational purposes only. Unauthorized use of this tool to monitor or log the activity of another individual without their consent is illegal and unethical. Always obtain explicit permission before deploying monitoring tools.

## Contact

For any questions or suggestions, feel free to reach out:

- **Name:** Shobhit Tomer
- **Email:** shobhittomer0810@gmail.com
- **LinkedIn:** [Shobhit Tomer](https://www.linkedin.com/in/shobhit-tomer-421841251/)
