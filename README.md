# pneumonia_detector

**Background**
- This is our project for altREU: Design, Program, and Use Computers to Benefit Society.
- Pneumonia is a leading cause of death worldwide, and the number one cause of mortality for children caused by an infectious disease.
Chest X-rays are vital in detecting and diagnosing pneumonia, and are one of the most ordered radiological reports, but there is a disproportionate lack of radiology specialists to interpret these X-ray images.
We present a tool which implements a convolutional neural network and interprets chest X-ray images and provides a pneumonia diagnosis.
Our goal is to provide a tool to assist medical professionals in diagnosing pneumonia using chest X-ray images, which is often difficult to interpret due to the great subtleties in radiological features between healthy and infected lungs.
**Approach**
We use the Chest X-ray Dataset with Lung Segmentation, found on PhysioNet, which is a large dataset of segmented X-ray images derived from the MIMIC-CXR-JPG dataset.
The program will take a lung X-ray image of a patient as input and output whether that patient has pneumonia and the degree to which it is certain of its decision.
To serve its purpose as an assisstive tool to medical professionals, the program also outputs a heatmap highlighting the regions of interest to the model in its diagnosis, implemented using Gradient-weighted Class Activation Mapping (Grad-CAM).
Upon experimenting with implementations built using TensorFlow and PyTorch, we found that fastai on Python is the most intuitive and powerful tool for our project.
