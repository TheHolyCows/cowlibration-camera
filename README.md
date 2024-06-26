# Cowlibration: Camera
This is a tool to calibrate your camera's intrinsics using a ChArUco board.

## Guide
### Clone repository
```
$ git clone https://github.com/TheHolyCows/cowlibration-field
```

### Install Python dependencies
```
$ pip install -r requirements.txt
```

### Usage
1. Prepare a ChArUco board with 5x5 1000 ArUco markers
    * See [https://github.com/TheHolyCows/cowlibration-board](https://github.com/TheHolyCows/cowlibration-board)
2. Record a video of the calibration board
3. Run camerea calibrator
```
$ python calibrate.py                \
    [input video]                    \
    [output camera model]            \
    --square [square size in inches] \
    --marker [marker size in inches] \
    --width [board width]            \
    --height [board height]
```

## Example
```
$ python calibrate.py          \
    [input video path]         \
    [output camera model path] \
    --square 0.709             \
    --marker 0.551             \
    --width 12                 \
    --height 8
```
