# Yolo-R DeepSort

- This repository was built by combining Yolo-R object detection and Deepsort algorithm.

## Installation
1. First, clone the repository.
```python
git clone https://github.com/chunmusic/Yolo-R_DeepSort
```

2. Create Python virtual environment based on Python 3.8
```python
conda create -n py38 python=3.8
```
3. Activate Python 3.8 virtual environment
```python
conda activate py38
```
4. Install required dependencies. 
```python
conda install pytorch torchvision cudatoolkit=11.1 -c pytorch -c conda-forge

pip install Cython numpy

pip install -r requirement.txt
```
5. Download yolor weight file (.pt) from [yolor_p6.pt](https://drive.google.com/file/d/1Tdn3yqpZ79X7R1Ql0zNlNScB1Dv9Fp76/view?usp=sharing)



## How to use

**Inference**
* Run the following command to test inference with video file.

```python
python detect.py --source walk.mp4 --cfg cfg/yolor_p6.cfg --weights yolor_p6.pt --conf-thres 0.25 --img-size 1280 --device 0 --view-img
```

## Screenshot

![Image1](https://raw.githubusercontent.com/chunmusic/Yolo-R_DeepSort/master/screenshot.gif)

## Reference

* [yolor](https://github.com/WongKinYiu/yolor)  
* [Yolov5_DeepSort_Pytorch](https://github.com/mikel-brostrom/Yolov5_DeepSort_Pytorch)   
* [deep_sort](https://github.com/nwojke/deep_sort)   
