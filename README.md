[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/9NCpqSMm)

# Step Detection and Classification for Different Cardio Machines

Our project aims to classify three distinct cardio activities—stair master, incline treadmill, and stationary bike—based on sensor data.

## Sensors and Data Collection

### Sensors
- Primary: Accelerometer
- Secondary: Gyroscope to capture rotational motion, essential for biking and exploratory for stair master or incline treadmill. 

### Device Placement
Phones will be strapped to the thigh for consistent and reliable signal capture.

### Data Collection Plan
- Each team member will record 5–10 minutes of activity per cardio machine in SensorLogger, ensuring sufficient data for training and testing.
- Recordings will be labeled with machine type and participant using the SensorLogger app.

### Data Cleaning
- Initial and terminal noise will be removed by trimming the first and last 5 seconds of each recording.
- Labeled data will be merged into a single dataset for feature extraction and modeling.

## Feature Engineering
We will extract features from both time-domain and frequency-domain data to differentiate activities effectively.
### Time-Domain Features
- Mean, variance, and quartiles of acceleration and gyroscopic data.
- Time between peaks (for activities with repetitive patterns).
### Frequency-Domain Features
- Dominant frequency and signal energy to identify rhythmic patterns.
- Spectral entropy for variability in motion.

## Analysis and Investigation
- Comparison of sensor configurations: Accelerometer-only vs. Accelerometer+Gyroscope.
- Performance evaluation: Confusion matrices to assess classification accuracy.
- Feature importance: Visualizations to highlight key features for distinguishing between cardio machines.
