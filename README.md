# OpenPose

Main Reference: https://github.com/ildoonet/tf-pose-estimation.git

This documentation had been prepared by assuming you had installed the dependencies of tensorflow-gpu and CUDA. If you haven’t install them, please refer to my github link for more information ( https://github.com/JJLim99/Implementation-of-TensorFlow-GPU-CUDA-in-Windows.git )
<br/><br/>
The code is tested using tensorflow-gpu=1.15 and keras=2.3.1, AMD Ryzen 5 3550H, 12GB RAM, GTX 1650

If you have error by running the original python scripts from the reference repo, can refer to mine.

Changes that made by me are:

1. Add the following lines into the python scripts:
import os
os.environ["CUDA_VISIBLE_DEVICES"] = "1"

2. Modify the code at line 27 
<br/>parser.add_argument('--camera', type=int, default=0) to parser.add_argument('--camera', type=str, default=0)

run_webcam.py is to test the OpenPose<br/>
people_count.py is to count the number of people
