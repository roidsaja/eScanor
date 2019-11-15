# eScanor
## electronic scan optical recognition
(the c in character isn't visible because you can't c it :p )

## overview
University final project for the curriculum subject named 'Interfacing 1'. Introducing briefly, eScanor allows an impaired vision individual to scan and read text from an A4 paper. It takes a snapshot of the image, converts to a txt file using OCR (Optical Character Recognition) and then speaks that converted text using TTS (Text-To-Speech).
It is designed to be as simple and minimal with minimum hassle for interaction, just a single push of a button will automatically trigger the procedure of scanning,convert and speak.

## limitations
* Using the 5MP camera that were built for the RPi and it isn't monochrome. Therefore, many noises may come from the surroundings.
* Lighting and environment plays a crucial part of taking image and converting to plain text.
* Takes significant amount of time to scan and convert for lengthy worded paper.

## Utilities
* tts.sh -- Tests the speaker for tts and adjust different voices.
* test.sh -- Tests each component including camera.

## init
1. `sudo apt-get update`
2. `sudo apt-get install -y build-essential python-pip python-dev`
3. `sudo apt-get install -y tesseract-ocr flite`
#### optional
4. `crontab ./cronfile`

## testing the camera
[head to raspberrypi.org documentation site](https://www.raspberrypi.org/documentation/configuration/camera.md)
