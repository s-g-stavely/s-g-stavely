## How to use an android phone as a webcam

# Prerequisites

- An android phone with a decent camera
- Windows PC
- A USB cable to connect that phone to your PC
- A way of positioning your phone such that it can capture your face. I used a clamp to attach my phone to my monitor

# Setup steps

- (Optional step, recommended if you plan to use your phone only for this and nothing else) Perform a factory reset of your phone, put phone into silent mode
- Install the [Reincubate Camo](https://reincubate.com/camo/) app on your PC
- Install the [Android app](https://play.google.com/store/apps/details?id=com.reincubate.camo) on your android phone
- Follow the instructions in the apps to get the phone configured to transmit video
- Confirm you can open your video calling app and use Camo as a video source
- Install [Scrcpy](https://github.com/Genymobile/scrcpy) by downloading the windows executable and extracting it somewhere
- Run Scrcpy. You should be able to control your phone's screen with the mouse. Middle click to press the home button, Alt+P to lock the screen, right click to wake.
  

# Daily process to use the webcam
- Launch the windows Camo app
- Launch Scrcpy and use it to open the phone Camo app
- Make your video call
- When finished, in Scrcpy press Alt-P to lock the screen