# casa0018dl4sn
# Snoring Detection with Edge Impulse

This project uses the Edge Impulse machine learning platform to develop a snoring detection system. It's implemented on an Arduino board equipped with a microphone. The system captures audio data, processes it through a machine learning model to detect snoring, and activates a buzzer if snoring is detected.

## Prerequisites

Before you start, ensure you have the following:

- An Arduino board with microphone support, such as **Arduino Nano 33 BLE Sense**.
- Arduino IDE installed on your computer.
- An active account on Edge Impulse with a project configured for audio processing.

## Installation

Follow these steps to get the project set up:

### Clone the Repository

Clone this repository to your local machine:

```bash
git clone <https://github.com/liangleiliu-lab/casa0018dl4sn.git>
```
Add this library ```ei-snoring_detection-arduino-1.0.8.zip``` through the Arduino IDE via: 

```Sketch > Include Library > Add .ZIP Library...```

Examples can then be found under:
```File > Examples > Snoring_Detection_inferencing``` 

Connect the microphone to your Arduino board. If using an Arduino Nano 33 BLE Sense, the microphone is built-in.

Attach a buzzer to the ```BUZZER_PIN``` specified in the code.

### Usage 

#### upload the code 
Connect your Arduino board to your computer, select the correct board and port from the Arduino IDE, and upload the sketch.

#### Running the Application

- Reset the board to start the detection process.
- The serial monitor in Arduino IDE will display inference results.
- The buzzer will sound if snoring is detected, depending on the detection confidence set in the source code.
## Edge Impulse Project Access

This project is powered by a machine learning model trained on the Edge Impulse platform. You can view and clone the project to adjust the model according to your specific needs.

### Access the Project

Visit the project's public page on Edge Impulse:

[Edge Impulse - Snoring Detection Project](https://studio.edgeimpulse.com/public/381731/live)

### Clone and Customize the Model

To clone and modify the project:

1. **Create an Account on Edge Impulse**:
   If you don't already have an Edge Impulse account, you'll need to create one. Visit [Edge Impulse](https://www.edgeimpulse.com) and sign up.

2. **Clone the Project**:
   - Once logged in, go to the [project page](https://studio.edgeimpulse.com/public/381731/live).
   - Click **Fork Project** to create a copy of the project under your account.

3. **Modify the Model**:
   - You can adjust the dataset, retrain the model, or tweak the DSP (Digital Signal Processing) parameters based on your requirements.
   - After modifying the model, you can deploy it by generating a new Arduino library from the **Deployment** tab.

4. **Update Your Local Repository**:
   - Download the updated Arduino library for your newly trained model.
   - Replace the existing library in your Arduino project with the new one.

### Re-deploy the Model

After you've adjusted and retrained the model on Edge Impulse:

- Follow the deployment steps provided in Edge Impulse to export the model to your Arduino device.
- Test the new model by uploading the updated code to your Arduino and observing the results via the serial monitor.

## Troubleshooting

Ensure your model's performance metrics meet your requirements before deploying it to your device. If you encounter issues with model accuracy or performance, consider:

- Adding more diverse training data.
- Increasing the complexity of the model (be aware of your device's hardware limitations).
- Revisiting feature extraction and signal processing techniques.


For further assistance, refer to the [Edge Impulse documentation](https://docs.edgeimpulse.com) or seek help from the Edge Impulse community forum.

## Project Report and Insights

For a comprehensive overview of the project, including the initial inspiration, development processes, deployment strategies, and detailed discussions on performance, you are encouraged to read the project report.

### View the Project Report

The report is available on GitHub and provides detailed documentation of the project lifecycle, challenges faced, and the solutions implemented. It can serve as a valuable resource for understanding the project in depth and for users looking to replicate or build upon this work.

[Read the Full Report Here](https://github.com/liangleiliu-lab/casa0018dl4sn/blob/main/casa0018_assessment_report_liangleiliu.pdf)

### Highlights from the Report

- **Project Inspiration**: Learn about what drove the creation of this snoring detection system.
- **Development Process**: Detailed explanation of the development steps, including model training and software development.
- **Deployment and Performance**: Analysis of the deployment strategies used and the performance metrics of the deployed model.

### Further Reading

This document is intended for those who are interested in the deeper technical aspects of the project or who may be conducting similar projects. It is also useful for academic purposes or for stakeholders looking to evaluate the project's efficacy.


## Acknowledgements

- **Edge Impulse Inc.** - For providing the machine learning platform that was instrumental in developing the snoring detection model.


