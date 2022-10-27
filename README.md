# Final-project
**Title of project and names of team members**:

Crop Classification and Crop phenology detection using deep learning and radar observations. 

I will do the project individually. 

**What problem do you want to work on?**
I am going to use satellite observations (radar backscatter time series) to classify crops and also detect crop phenology (crop growth cycle) using radar images (backscatter time series). 
I will work with images from satellite and will compare two different deep learning approaches, Convolutional neural network and transformers for crop classification and phenology detection. 
I aim to connect this project to a special issue in Remote Sensing of Environment Jouranl ( one of the best journals among engineering journals with impact factor 13). the title of the special issue is “advancing deep learning for time series analysis”. As the Satellites are able to measure and observe regularly with a specific revisit time for example every 12 days, it is possible to access to the satellite observations as a time series and deep learning is a powerful technique to analyze the time series to detect the crop growth cycle over time or even to classify the crop. 
 

**What are the existing works that are most relevant to your problem?**
There are several recent studies in which different Machine learning and Deep learning techniques (random forest, support vector machine, fully connected multilayer perceptron (MLP) and convolutional neural network) have been used with L-band and C-band SAR observations for crop classification and crop phenology detection. However, transformers has not been used for this application yet. Please see the following papers:

•	Huang, Xiaodong, Michele Reba, Alisa Coffin, Benjamin RK Runkle, Yanbo Huang, Bruce Chapman, Beth Ziniti et al. "Cropland mapping with L-band UAVSAR and development of NISAR products." Remote Sensing of Environment 253 (2021): 112180.

•	Kussul, Nataliia, Mykola Lavreniuk, Sergii Skakun, and Andrii Shelestov. "Deep learning classification of land cover and crop types using remote sensing data." IEEE Geoscience and Remote Sensing Letters 14, no. 5 (2017): 778-782.

•	Bargiel, Damian. "A new method for crop classification combining time series of radar images and crop phenology information." Remote sensing of environment 198 (2017): 369-383

**What dataset will be used for training and evaluation?** Provide detailed description.
For crop classification I will use the CDL data set for training and evaluation of the model. The CDL is produced using observations from various space borne platforms such as Landsat8 and Sentinel2 provided on 30*30 m grids and encompasses 106 different crops. CDL accuracy with respect to ground truth is estimated to be in the 85%-95% range for major crop types. There are several studies that have used CDL as the training dataset.
Moreover, NASA research team has conducted several field campaigns in the corn fields in Iowa in 2016 that the data is available to use. 
I have also done a field measurement in three corn and soybean fields from June to October 2022 to measure the crop phenology (measuring the height, number of leaves and vegetation water content). I am going to use this data to determine vegetation water content from radar time series. As the measurement is not large I have the plan to use this data with the Iowa data (2016) mentioned above. However, I am looking to find more data in future. 

**What are the metrics for evaluation? How will you compare different solutions or know if your model is working?**
I will use the insitu measurements for crop classification and phenology of the crop as the evaluation dataset. So, the model is a classification model and a correct prediction of the crop at the end of the simulation is representing that the model is working well. 

**What computational resources will you use? GitHub Codespaces, Colab, MSU HPCC or other resources?**
I will use python on HPCC
