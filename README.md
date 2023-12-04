# Bonsai-Regression-Rescue

A repo tailored to support [Bonsai's](https://github.com/microsoft/EdgeML/tree/master) regression capabilities. I've wrestled with it so you won't have to.

## Data Setup


### 1. Organize Your Data

Split your data into training and testing sets, saving them as `train.npy` and `test.npy`. Organize your files within a dedicated folder for clarity.
```
your_data_folder/
|-- train.npy
|-- test.npy
```

Initialize the `DataDir` variable in your code to point to the path where your data resides. 
```
DataDir = 'path/to/your_data_folder'
```

### 2. Data Format

Take note that Bonsai treats the first column of your data as the target variable. Ensure your data is formatted accordingly, placing the target variable in the first column.
