
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

```bash
python detect.py --weights yolov5s.pt --source data/images/bus.jpg
## To test on other images: Download image of interest into "yolov5/data/images" and run the same command as above, but change the last part (bus.jpg) accordingly
## For example python detect.py --weights yolov5s.pt --source data/images/car.jpg
```

