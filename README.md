# Car Trajectory Prediction at an Intersection Using LSTM Model
This project uses an LSTM (Long Short-Term Memory) model to predict car trajectories at a traffic intersection in the city of Coldwater. The video used for this project is a YouTube live-stream of the city of Coldwater (https://www.youtube.com/watch?v=ByED80IKdIU).


The project is divided into three main phases, each managed by a Google Colab notebook:
1. Data Acquisition: Processing of the video of a busy intersection to extract car trajectories.
2. Data Cleaning: Analyzing and cleaning the extracted data to obtain an accurate dataset.
3. Dataset Creation and Model Training: Creating a dataset with the cleaned data and training an LSTM model.

# Methodology
In this project, I developed and tested two different approaches to predict car trajectories at the intersection:

1. Total Model Approach: A single LSTM model (total_model) was developed to predict any car trajectory at the intersection.
2. Directional Models Approach: Four separate LSTM models were developed, each specialized in predicting trajectories for cars entering the intersection from a specific direction (North, South, East, West).

# Folders
1. Models: in this folder there are the latest models developed
2. Dataframes: in this folder there are the some dataframes used for the creation of the dataset and training, the number after the dataframe name is the number of trajectories of each kind (see the code comments for more info)
3. Trajectories: contains the trajectories before and after the cleaning process
4. Videos: contains the videos used for the data acquisition and testing, in the folder "videos/processed/" there are some of the result obtained by the networks. Note that the videos that have been processed by the "total model" or the "four models" are labelled as "total_model_prediction" and "four_models_prediction". If the video name contains "_all_frames" it means that in this video processing all the video frames where used.

# Results
You can find video results in the "videos/processed/" folder
![incrocio_test_four_models_prediction_all_frames-ezgif com-video-to-gif-converter (1)](https://github.com/AntonLissa/trajectory_prediction/assets/168411880/f6dbae4f-ecfb-409b-a642-d07510b5f1d5)
![Screenshot 2024-06-12 155206](https://github.com/AntonLissa/trajectory_prediction/assets/168411880/5ef4bd68-0aff-4445-af99-3fc10d4e322d)

# Inspiration
This project was inspired by the article "Real-Time Vehicle Trajectory Prediction for Traffic Conflict Detection at Unsignalized Intersections", you can find it here: https://doi.org/10.1155/2021/8453726
