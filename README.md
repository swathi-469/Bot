# pose-estimation-detection

Pose estimation & detection has been minimally implemented using the OpenPose implementation https://github.com/ildoonet/tf-pose-estimation with Tensorflow. For the binary classification of poses, namely the classes : sitting or standing, the model used, MobileNet (a CNN originally trained on the ImageNet Large Visual Recognition Challenge dataset), was retrained (final layer) on a dataset of ~1500 images of poses.

The model is able to estimate the human poses as well as classify the current pose to a fairly good degree of accuracy.

### Demo

**An alternative for improving the model along with deep learning is to include heuristics, in the form of calculation of the skeletal points’ relative distances from each other.**

 **FPS & estimation/detection varies with the CPU/GPU power.**
 
### Training Examples

- For sitting pose
![alt text](/images/sitting.jpeg)

- For standing pose
![alt text](/images/standing.jpeg)

### Dependencies

The following are required :

- python3
- tensorflow 1.9.0 (works well even with CPU version)
- opencv3
- slim
- slidingwindow
  - https://github.com/adamrehn/slidingwindow

### Cloning & installing dependencies

```bash
$ git clone https://github.com/SyBorg91/pose-estimation-detection
$ cd pose-estimation-detection
$ pip3 install -r requirements.txt
```




