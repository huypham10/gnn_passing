# My MSc. final project on measuring risk and reward of passing using Statsbomb's Open 360 data.

## The raw data source for this project can be found here: https://github.com/statsbomb/open-data/tree/master/data. (Only matches from Men's Euro 2020 were included)

## There are 4 Jupyter Notebook used for this project. These have been ordered accordingly. They follow the work flow laid out in the report.

1. The first Jupyter Notebook extracts data from source files to generate all features and outputs the master_data.json file for handcrafted features (used in the second Jupyter Notebook), and tracking_data.json file for graph representations (used in the third Jupyter Notebook).

2. The second Jupyter Notebook uses master_data.json file to perform EDA and train the logistic regression model, and output a master_data_training.json file to be used for training the GNN (third Jupyter Notebook); and a master_data_analysis.json to be used for application demonstration (the fourth Jupyter Notebook).

3. The third Jupyter Notebook uses tracking_data.json and master_data.json files to generate a graph representation for each pass (each pass is a .pt file), and use those representations to train the GNN. 

4. The fourth Jupyter Notebook uses master_data_analysis.json to perform analyses.

Only graph representation .pt files have been uploaded to https://github.com/huypham10/gnn_passing, since all other .json files are too heavy for github.