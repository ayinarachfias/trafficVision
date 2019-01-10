# Traffic Vision
This app detects cars/buses in a live traffic using deep learning network Yolo-V2. It has been optimized for AMD-GPUs using MIVisionX.

![Traffic Vision Animation](media/traffic_viosion.gif)

## Features
1. Detection of vechicle with bounding box
1. Detection of vehicle direction of travel
1. Prediction the speed of the vehicle
1. Prediction of approximate vehicle size

## How to Run

### Use Model
<img src="media/speed_detection_user_interface.jpg" width=600>

### Demo

Demo uses a recorded video in the media dir
```
% ./main.py
('Loaded', 'yoloOpenVX')
OK: loaded 22 kernels from libvx_nn.so
OK: OpenVX using GPU device#0 (gfx900) [OpenCL 1.2 ] [SvmCaps 0 1]
OK: annCreateInference: successful
Processed a total of  102 frames
OK: OpenCL buffer usage: 87771380, 46/46
%
```
### Other Examples

**recorded video**
> 1. ./main.py --video <path-to-video>/vid.mp4
  
**traffic cam ip** 
> 2. ./main.py --cam_ip 'http://166.149.104.112:8082/snap.jpg'

## Installation

### Prerequisites 

1. GPU: Radeon Instinct or Vega Family of Products with [ROCm](https://rocm.github.io/ROCmInstall.html) and OpenCL development kit
1. [Install AMD's MIVisionX toolkit](https://gpuopen-professionalcompute-libraries.github.io/MIVisionX/) : AMD's MIVisionX toolkit is a comprehensive computer vision and machine intelligence libraries, utilities
1. [CMake](http://cmake.org/download/)
1. [Google's Protobuf](https://github.com/google/protobuf)

### Steps

> git clone https://github.com/srohit0/trafficVision
> 

## Design

### High Level
<img src="media/speed_detection_top_level_arch.jpg" width="600">

### Modules
<img src="media/speed_detection_modules.jpg" width="600">

### Dependencies

## Development

### Model Conversion
<img src="media/speed_detection_model_conversion.jpg" width=680>




<img src="media/speed_detection_infrastructure.jpg" width=480>


## Credit
* **Schmitt, Mike**
* **Nagesh gowda, Kiriti**
* **Rawther, Rajy**
