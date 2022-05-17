This is a 2D object detection trained with YOLOR for Infrared images 
The dataset is obtained from FLIR teledyne :
https://www.flir.in/oem/adas/adas-dataset-form/

It contains the 15 categories ,
	
Person
Bike
Car
Motorcycle
Bus
Train
Truck
Traffic light
Fire Hydrant
Street Sign
Dog
Skateboard
Stroller
Scooter
Other Vehicle

The dataset has used the COCO format that has 80 classes and all these 15 categories id has been mapped according to their coco dataset .Labels are available in the json format and you have to write a script file to generate the ground truth in YOLO format( class id,x,y, w, h)
Regarding the train, test and validation split, The dataset has been split already and is available in FLIR portal.

Most importantly for training only the thermal images were used

YOLOR TRAINING :
Trained the model from scratch without any pretrained models and model parameters were retained . I have used the NVIDIA environment which provides 4 TESLA T4 cores. Becuase of rescource limitation , can able to train only for 10 epochs .
EPOCHS : 10 

Results are available in resource folder 
