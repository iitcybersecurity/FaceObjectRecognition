# FaceObjectRecognition
Darknet YOLOv3 trained with OpenImages dataset using the classes 1-Human head 2- Mobile phone.

How to use:

Step 1: Download and build Darknet Yolo
git clone https://github.com/pjreddie/darknet
cd darknet
make

Step 2: Configure network 
copy data/head_smartphone.data in darknet/data
copy data/head_smartphone.names in darknet/data
copy cfg/head_smartphone.cfg in darknet/cfg
copy backup/head_smartphone_900.weights in darknet/backup

Step 3: Testing command: 
./darknet detector test cfg/head_smartphone.data cfg/head_smartphone.cfg backup/head_smartphone_900.weights <IMAGE_PATH> 

