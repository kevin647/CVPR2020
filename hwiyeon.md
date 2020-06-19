### Predicting Semantic Map Representations From Images Using Pyramid Occupancy Networks
- **Oral presentation** [(Video)](http://d1tz9o43mm5y8k.cloudfront.net/CVPR20/CVPR20/2361/2361-oral.mp4)

- Contributions
    - It proposed a method to generate birds-eye-view semantic map by monocular images
    
- Overview
    - ![semantic_map_overview](./img/semantic_map_overview.png)
    
- Method
    - ![semantic_map_network](./img/semantic_map_network.png)
    - Use dense transformer layer
    - Introduce pyramid occupancy network
    - Use semantic occupancy grids
            
- Results
    - ![semantic_map_results](./img/semantic_map_results.png)

### Vision-Language Navigation With Self-Supervised Auxiliary Reasoning Tasks
- **Oral presentation** [(Video)](http://d1tz9o43mm5y8k.cloudfront.net/CVPR20/CVPR20/4322/4322-oral.mp4)

- Contributions
    - It proposed a method for vision-language navigation which solves auxiliary tasks to take advantage of the additional training signals derived from the semantic information.
    
- Overview
    - ![aux_RN_overview](./img/aux_RN_overview.png)

- Method
    - ![aux_RN_network](./img/aux_RN_network.png)
    - Auxiliary tasks
        - Trajectory retelling 
        - Progress estimation
        - Cross-modal matching
        - Angle predictions
    - Graph map
        - Jointly use imitation learning and reinforcement learning for the navigation
    
- Results
    - ![aux_RN_results](./img/aux_RN_results.png)