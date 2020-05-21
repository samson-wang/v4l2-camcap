# To capture mjpeg video from webcam

## Reference:

http://jwhsmith.net/2014/12/capturing-a-webcam-stream-using-v4l2/

https://gist.github.com/sammy17/b391c68a91f381aad0d149e325e6a87e

```
g++ -Wall -o webcam_capture webcam_cap.cpp

# To capture video from /dev/video0, 150 frames, save into test.mjpeg
./webcam_capture /dev/video0 test.mjpeg 150

ffplay -f mjpeg test.mjpeg
```
