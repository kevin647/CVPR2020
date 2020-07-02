### SurfelGAN: Synthesizing Realistic Sensor Data for Autonomous Driving
- **Oral presentation** [(Video)](http://cvpr20.cn/CVPR20/CVPR20/6266/6266-oral.mp4)

- Goal
    - Generating realistic scenario sensor data, based only on a limited amount of lidar and camera data collected by an autonomous vehicle
    
- Overview
    - ![SurfelGAN1](./img/SurfelGAN1.PNG)
    - paired data: real&generated pair. unpaired data: only generated data or only real data
    
- Method
    - ![SurfelGAN2](./img/SurfelGAN2.PNG)
    - ![SurfelGAN3](./img/SurfelGAN3.PNG)
    - collect real world sensor data from A->B trajectory
    - reconstruct real world by using collected sensor data(C->D) with surfel.
    - when reconstructing, use GAN method to close the domain gap between real world and generated data
        
- Experiments
    - ![SurfelGAN_exp1](./img/SurfelGAN_exp1.PNG)
    - ![SurfelGAN_exp2](./img/SurfelGAN_exp2.PNG)
    - ![SurfelGAN_exp3](./img/SurfelGAN_exp3.PNG)
    - ![SurfelGAN_exp4](./img/SurfelGAN_exp4.PNG)


### SurfelGAN: Synthesizing Realistic Sensor Data for Autonomous Driving
- **Oral presentation** [(Video)](http://cvpr20.cn/CVPR20/CVPR20/1217/1217-1min.mp4)

- Goal
    - jointly perform perception and motion prediction from 3D point clouds
    
- Overview
    - ![MotionNet1](./img/MotionNet1.PNG)
    - cell classification: category of each cell (ex vehicle, pedestrian or background)
    - motion prediction: future trajectory of each cell
    - state estimation: the current motion status of each cell (static or moving)
    
- Method
    - ![MotionNet2](./img/MotionNet2.PNG)
    - Use spatio-temporal convolution as building block
    - T: temporal dimension(time), C: the number of cell categories, W, H: probability coordinates of data, N: number of future frame
    - cell classification's output: C x H x W
    - motion prediction's output: N x H x W x 2 (2: start & end)
    - stat estimation's output: H x W
- Loss
    - ![MotionNet3](./img/MotionNet3.PNG)
    - predicted motions should be very close without much divergence in a rigid object
    - ![MotionNet4](./img/MotionNet4.PNG)
    - there will be no sharp change of motions between two consecutive frames
    - ![MotionNet5](./img/MotionNet5.PNG)
    - Lft mainly operates on the foreground objects, such as vehicles, and does not consider the background cells
    - ![MotionNet6](./img/MotionNet6.PNG)
    - Lcls, Lstate: cross-entropy losses for the cell classification and state-estimation heads
    - Lmotion : smooth L1 loss for the motion-prediction head
    - α, β and γ : weighting hyperparameters(balancing factors)
    
- Experiments
    - ![MotionNet_exp1](./img/MotionNet_exp1.PNG)
    - ![MotionNet_exp2](./img/MotionNet_exp2.PNG)
