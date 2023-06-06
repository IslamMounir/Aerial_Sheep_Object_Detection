# Aerial Sheep Object Detection

This project aims to detect sheep in aerial images using an object detection model. The model is trained on aerial sheep dataset. The objective is to accurately identify and localize the sheep within the images.

## Dataset

The dataset contains images taken from a birds-eye view with instances of sheep in them. Images do not differentiate between gender or breed of sheep, instead grouping them into a single class named "sheep".

Here are some sample images from the dataset:

<br/>
<div align="center">
  <img src="https://github.com/IslamMounir/Aerial_Sheep_Object_Detection/blob/main/images/dataset_1.jpg" alt="Dataset Sample 1" width="200"/>
  <img src="https://github.com/IslamMounir/Aerial_Sheep_Object_Detection/blob/main/images/dataset_2.jpg" alt="Dataset Sample 2" width="200"/>
  <img src="https://github.com/IslamMounir/Aerial_Sheep_Object_Detection/blob/main/images/dataset_3.jpg" alt="Dataset Sample 3" width="200"/>
  <img src="https://github.com/IslamMounir/Aerial_Sheep_Object_Detection/blob/main/images/dataset_4.jpg" alt="Dataset Sample 4" width="200"/>
</div>

## Model Training

The object detection model is trained using the YOLOv5 model architecture.
The model is trained to accurately identify and locate the sheep within the images. 
The training is performed for multiple epochs using the "train" and "valid" datasets  with the following configurations:
- Model: YOLOv5s
- Optimizer: SGD
- Image Size: 600
- Learning Rate: 0.01

The training results are as follows:
- Precision: 0.967
- Recall: 0.933
- mAP50: 0.967
- mAP50-95: 0.585



## Model Evaluation

The trained model was evaluated on the test dataset with the following results:
- Precision: 0.973
- Recall: 0.935
- mAP50: 0.969
- mAP50-95: 0.591


## Inference

The model was used to perform inference on a set of test images. Here are some sample images along with the predicted bounding boxes:

  <br/>
<div align="center">
  <img src="https://github.com/IslamMounir/Aerial_Sheep_Object_Detection/blob/main/images/test_1.jpg" alt="Inference Sample 1" width="200"/>
  <img src="https://github.com/IslamMounir/Aerial_Sheep_Object_Detection/blob/main/images/test_2.jpg" alt="Inference Sample 2" width="200"/>
  <img src="https://github.com/IslamMounir/Aerial_Sheep_Object_Detection/blob/main/images/test_3.jpg" alt="Inference Sample 3" width="200"/>
  <img src="https://github.com/IslamMounir/Aerial_Sheep_Object_Detection/blob/main/images/test_4.jpg" alt="Inference Sample 4" width="200"/>
</div>

## Usage

To use this project, follow these steps:

1. Clone the repository to your local machine.

2. Open the `train.ipynb` notebook.

3. Run the notebook to perform training, testing and inference. The notebook contains all the necessary code and instructions for each step.

4. Make sure to modify any relevant file paths or configurations within the notebook to suit your specific setup and requirements.

Feel free to explore and customize the code within the notebook to further adapt it for your needs.


## Acknowledgments

- The dataset used in this project was collected from a publicly available source. [Click here](https://universe.roboflow.com/riis/aerial-sheep) to access the dataset.

