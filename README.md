# Fire Detection System

## Project Overview
An advanced fire detection system completed in 2021, designed for both indoor and outdoor environments. The system utilized a specialized camera with an integrated edge device for real-time inference, identifying fire hazards and providing immediate visual alerts to improve safety and response times in various settings.

![Fire Detection System](https://placeholder-image.com/fire-detection-system)

## Role
AI Research Engineer in a 3-person cross-functional team (hardware, software, and AI engineers)

## Technologies Used
- **Model Architecture**: YOLOv3-tiny
- **Training Framework**: Darknet
- **Hardware**: Banana BPI-M3 edge device
- **Implementation**: C++ for detection code
- **Operating System**: Linux-based system
- **Optimization Techniques**: Quantization for improved inference speed

## Key Achievements

### Dataset Development
- Built a comprehensive dataset by combining open-source and self-recorded fire scenarios
- Collected over 100,000 images encompassing various fire scenarios and conditions
- Strategically augmented dataset to improve false positive handling
- Avoided reliance on color-based augmentation, which is ineffective for fire detection

### Model Implementation
- Successfully implemented YOLOv3-tiny model on resource-constrained Banana BPI-M3 hardware
- Trained the model using Darknet framework on a Windows system with dual GPU acceleration
- Applied quantization techniques to enhance inference speed for real-time detection
- Achieved optimal balance between detection accuracy and computational efficiency

### Problem Solving
- Resolved practical issues with false detections from similar visual patterns (welding sparks, bright lamps)
- Improved detection accuracy through systematic optimization
- Developed solutions that met Korea Fire Institute testing requirements
- Engineered a system capable of distinguishing actual fires from visually similar phenomena

### Hardware Integration
- Integrated the detection model with custom camera hardware featuring built-in edge processing
- Implemented visual alert system using LED indicators (green for normal conditions, red for fire detection)
- Ensured seamless operation between hardware and software components

## System Architecture

### Custom Camera and Edge Device
The system utilizes a custom-developed camera with an integrated edge device running on a Linux system. This unified design ensures robust and efficient real-time processing without requiring additional external hardware.

### Detection Algorithm
The fire detection algorithm is implemented in C++ to leverage the performance benefits of low-level programming, critical for real-time applications on edge devices with limited resources.

### Fire Detection Model
The three-layer YOLOv3-Tiny model was selected for its balance between detection accuracy and computational efficiency. Training was conducted on a Windows system equipped with 2 GPUs to accelerate the process.

### Alert System
The camera features a built-in LED lamp that provides immediate visual feedback. The LED remains green under normal conditions and switches to red upon detecting fire, ensuring clear and instant alerts.

## Research Publication
**Paper Title**: "An Improvement of the Fire Detection and Classification Method Using YOLOv3 for Surveillance Systems"  
**Published in**: MDPI Sensors, 2021  
**Role**: Co-first author  
**Key Contributions**:
- Presented optimized fire detection methodology for surveillance applications
- Demonstrated improved accuracy and performance in real-world scenarios
- Validated the approach through rigorous testing and analysis

## Challenges and Solutions

### Challenge: Inconsistent Visual Patterns of Fire
**Solution**: Unlike objects with consistent shapes or specific colors, fire presents varying visual patterns. To address this, we collected an extensive dataset of over 100,000 images, encompassing various combinations and potential fire scenarios.

### Challenge: False Positives from Similar Visual Patterns
**Solution**: We implemented strategic dataset augmentation to train the model to distinguish between actual fires and visually similar phenomena like welding sparks and bright lamps.

### Challenge: Resource Constraints of Edge Devices
**Solution**: Applied model quantization and optimization techniques to ensure efficient operation on the Banana BPI-M3 hardware while maintaining detection accuracy.

### Challenge: Addressing Industry Standards
**Solution**: Worked with Korea Fire Institute requirements to understand the rigorous standards for fire detection systems and inform our development approach.

## Project Completion
This project was completed in 2021. The fire detection system met our internal design specifications and the research and development from this project contributed valuable insights to the field of computer vision-based fire detection systems.

## Contact Information
While this project was completed in 2021, I'm happy to discuss the technical approaches, methodologies, and lessons learned.
