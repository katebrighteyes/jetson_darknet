# jetson_darknet

mkdir weights

cd weights

wget https://pjreddie.com/media/files/yolov2.weights

wget https://pjreddie.com/media/files/yolov3.weights

wget https://pjreddie.com/media/files/yolov3-tiny.weights

wget https://pjreddie.com/media/files/yolov2-tiny.weights

-----------------------------------------------------------------------

./darknet detector demo cfg/coco.data cfg/yolov3.cfg weights/yolov3.weights ./mov/Driving.mp4 

./darknet detector demo cfg/coco.data cfg/yolov3.cfg weights/yolov3.weights -c 0

./darknet detector demo cfg/coco.data cfg/yolov2-tiny.cfg weights/yolov2-tiny.weights ./mov/Driving.mp4 

./darknet detector demo cfg/coco.data cfg/yolov2-tiny.cfg weights/yolov2-tiny.weights -c 0
