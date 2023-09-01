# Data Cleaning and Model Training

- The [Melbourne city 2019 parking data](https://data.melbourne.vic.gov.au/explore/dataset/on-street-car-parking-sensor-data-2019/information/) is used in our model.

- In the data, parking information is given for each specific parking slot. We grouped them according to their segment_id s obtained which can be found ['here'](https://data.melbourne.vic.gov.au/explore/dataset/on-street-parking-bays/table/).

- This data also contains coordinates of each bay. After grouping them, we obtained the starting and ending coordinates of segments and used those results in our algorithm to find the nearest 10 segments.

### The layout of project folder/file structure
```
├── Model
│   ├── public
│   ├── ann_implementation.ipynb
│   ├── conv1d.ipynb
│   ├── Model_LSTM_10min.ipynb
│   ├── Model_LSTM_30min_later.ipynb
│   ├── Model_LSTM_30min_later.ipynb
│   ├── mongo_save.ipynb
│   ├── mongo_save2.ipynb
│   ├── mongo_save3.ipynb
│   ├── naive_model.ipynb
│   ├── read_some_things.ipynb
├── dataCleaning
-> ecemin segments branchi altındaki dataCleaning/createdFilesEcem/segments dosyası atılacak
├── maps
├── pickles
│   ├── src
│   ├── src
│   ├── src
│   ├── src
│   ├── src
│   ├── src
│   ├── src
│   ├── src
│   ├── src
│   ├── src

├── .gitignore
└── README.md
```
#### **Frontend side**
##### `ann_implementation.ipynb`
  - Artificial Neural Network implementation to train the model
  - This is not completed 
##### `conv1d.ipynb`
  - Convolutional 1D Neural Network to train the model
  - Only for one segment
  - Not efficient enough -> root mean abs error around 0.1 for only 1 step ahead prediction
##### `Model_LSTM_10min.ipynb`
  - Instead of 5 min intervals, 10 min intervals are taking into account
##### `Model_LSTM_30min_later.ipynb`
  - For one segment by using 5 min intervals 6 step ahead prediction old version
  - Attempt to train the model
##### `mongo_save.ipynb`
  - Mongo_save_x.ipynb files are used to put the obtained data to our mongodb
##### `naive_model.ipynb`
  - 1 week before data is used
##### `read_some_things.ipynb`
  - Use segment and their coordinate values to plot them on the map
