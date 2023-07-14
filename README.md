Student Verification Code

# Generating a QR code

## Prerequisites
- Python 3.x installed on your system
- `qrcode` library installed (`pip install qrcode`)

## Installation
1. Clone this repository or download the `student_verification_code.py` file.
2. Install the required dependencies by running the following command:
   ```
   pip install qrcode
   ```

## Usage
1. Enter the student data for the QR code when prompted.
2. The script will generate a QR code based on the entered data and save it as `Student_QR.jpg` in the same directory.


# Student Verification Code

This is a Python script that performs student verification based on a QR code. It uses the `cv2` library for image processing, the `pyzbar` library for QR code decoding, and the `PIL` library for image loading. The script also relies on a student database stored in a JSON file.

## Prerequisites
- Python 3.x installed on your system
- `cv2`, `pyzbar`, and `PIL` libraries installed (`pip install opencv-python pyzbar pillow`)

## Installation
1. Clone this repository or download the `student_verification_code.py` file.
2. Install the required dependencies by running the following command:
   ```
   pip install opencv-python pyzbar pillow
   ```

## Usage
1. Create a JSON file named `student_database.json` in the same directory as the script.
2. Populate the `student_database.json` file with student data in the following format:
   ```json
   {
     "qr_code_data_1": {
       "roll": "123456",
       "name": "John Doe",
       "class": "10th Grade",
       "address": "123 Main St, City"
     },
     "qr_code_data_2": {
       "roll": "789012",
       "name": "Jane Smith",
       "class": "12th Grade",
       "address": "456 Elm St, Town"
     },
     ...
   }
   ```
3. Save a QR code image named `Student_QR.jpg` in the same directory as the script. The QR code should correspond to one of the student entries in the `student_database.json` file.
4. Open a terminal or command prompt and navigate to the directory where the `student_verification_code.py` file is located.
5. Run the following command:
   ```
   python student_verification_code.py
   ```

After saving the QR code image as `Student_QR.jpg` and populating the `student_database.json` file with the student data, we can run the script. The script will read the QR code, verify the student against the database, and display the student information if found.

```
QR Code Data: qr_code_data_1
Roll no.: 123456
Student Name: John Doe
Class: 10th Grade
Address: 123 Main St, City
```





