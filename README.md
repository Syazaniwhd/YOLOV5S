This is an updated version of Yolov5 algorithm which is now able to do Object Detection in on any locally downloaded images or videos.
It can also conduct real time Object Detection


However, this algorithm can only detect the 80 classes from coco.names training set and have not been tested on a custom training set yet.


For a video tutorial refer to this link: https://www.youtube.com/watch?v=_rgRx2UpNzY

<details open>
<summary>Set up Virtual Environment</summary>
  
```bash
# From terminal or anaconda prompt
  conda create -n yolov5s python=3.9
  conda activate yolov5s
```


<details open>
<summary>Install</summary>

Clone repo and install [requirements.txt](https://github.com/ultralytics/yolov5/blob/master/requirements.txt) in a
[**Python>=3.7.0**](https://www.python.org/) environment, including
[**PyTorch>=1.7**](https://pytorch.org/get-started/locally/).

```bash
git clone https://github.com/ultralytics/yolov5  # clone
cd yolov5
pip install -r requirements.txt  # install
```

<details open>
<summary>Running Program</summary>

```bash
python detect.py --weights yolov5s.pt --source data/images/bus.jpg
## To test on other images: Download image of interest into "yolov5/data/images" in .jpg or .mp4 format
## Run the same command as above, but change the last part (bus.jpg to car.jpg or fish.mp4) accordingly
## For example python detect.py --weights yolov5s.pt --source data/images/car.jpg
## Change to source 0 for real time detection with webcam/camera
python detect.py --weights yolov5s.pt --source 0
```

