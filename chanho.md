### Conditional Channel Gated Networks for Task-Aware Continual Learning
- **Oral presentation** [(Video)](http://d1tz9o43mm5y8k.cloudfront.net/CVPR20/CVPR20/2376/2376-oral.mp4)

- Goal
    - It proposed a gating network for continual learning.
    
- Overview
    - ![ch1_overview](./img/ch1_overview.PNG)
    
- Method
    - ![ch1_network](./img/ch1_network.PNG)
    - Use a selected convolutional channel via gumbel-softmax
    - Freeze convolutional channels which are selected frequently
    - Regularizer: sparsity objective
        
- Experiments
    - ![ch1_exp1](./img/ch1_exp1.PNG)
    - ![ch1_exp2](./img/ch1_exp2.PNG)

### Maintaining Discrimination and Fairness in Class Incremental Learning
- [(Video)](http://d1tz9o43mm5y8k.cloudfront.net/CVPR20/CVPR20/8842/8842-1min.mp4)

- Goal
    - ![ch2_goal](./img/ch2_goal.PNG)
    - Maintain discrimation and fairness for incremental learning
    
- Overview
    - ![ch2_overview](./img/ch2_overview.PNG)

- Method
    - Knowledge distillation with rehearsal data
    - ![ch2_motivation](./img/ch2_motivation.PNG)
    - Align so that the last convolution parameters of each task has the same size norm
    
- Experiments
    - ![ch2_exp1](./img/ch2_exp1.PNG)
    - ![ch2_exp2](./img/ch2_exp2.PNG)
