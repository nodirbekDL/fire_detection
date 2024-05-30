# Fire Detection System

### Short Description
A fire detection system designed for both indoor and outdoor environments, utilizing a specialized camera with an integrated edge device for real-time inference. The system identifies fire hazards and provides immediate visual alerts.

### Key Features/Technologies
- **Custom Camera**: Developed by our company, featuring an integrated edge device that operates on a Linux system.
- **Detection Code**: Implemented in C++ for efficient processing.
- **YOLOv3-Tiny Model**: Employs a three-layer YOLOv3-Tiny model for fire detection.
- **Darknet Framework**: Used for training the detection model.
- **Quantization**: Applied to enhance the inference speed.
- **Visual Alerts**: The camera includes a built-in LED lamp that remains green under normal conditions and turns red upon detecting fire.

### Detailed Explanation

#### Custom Camera and Edge Device
- **Development**: The camera, developed in-house, features an integrated edge device running on a Linux system. This design ensures robust and efficient real-time processing.
- **Detection Implementation**: The detection algorithm is implemented in C++ to leverage the performance benefits of low-level programming.

#### Fire Detection Model
- **Model**: Utilizes a three-layer YOLOv3-Tiny model, selected for its balance between detection accuracy and computational efficiency.
- **Training Framework**: Darknet was employed for training the YOLOv3-Tiny model. The training was conducted on a Windows system equipped with 2 GPUs to accelerate the process.
- **Quantization**: Applied to the model to enhance inference speed, making it suitable for real-time detection on the edge device.

#### Visual Alerts
- **LED Indicator**: The camera features a built-in LED lamp that provides immediate visual feedback. The LED remains green under normal conditions and switches to red upon detecting fire, ensuring clear and instant alerts.

### Challenges and Learnings
Fire detection is inherently challenging due to the lack of consistent shapes or specific colors associated with fire. To address this, we collected an extensive dataset of over 100,000 images, encompassing various combinations and potential fire scenarios. This approach ensured robust training without relying on color-based augmentation, which is ineffective for fire detection.

### Screenshots/Media
![Fire Detection System Screenshot](link-to-screenshot)

### Link to Project/Repository
[GitHub Repository](https://github.com/username/fire-detection-system) | [Live Demo](https://username.github.io/fire-detection-system/)

### Paper Publication
We have published a paper on this work in an SCI journal, detailing the methodologies and findings of the fire detection system.

### Usage

#### Basic Usage
Once the system is installed and the camera is operational, it can monitor both indoor and outdoor environments for fire hazards. The integrated edge device processes detections in real time, triggering visual alerts via the LED lamp on the camera.

#### Configuration
The system allows for customization of detection parameters to suit specific needs. Adjust detection thresholds, specify the sensitivity of the fire detection algorithm, and configure the LED alert settings.

#### Advanced Features
- **Real-time Monitoring**: The system continuously monitors the environment, providing instant visual feedback through the LED indicator.
- **Detailed Reports**: Generate reports on fire detection events to evaluate system performance and improve safety measures.
