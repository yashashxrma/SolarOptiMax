# SolarOptiMax: Solar Irradiance Prediction and Rooftop Area Calculation

This repository features Solar Irradiance Prediction and Rooftop Area Calculation models. They optimize solar panel installation by predicting irradiance and estimating rooftop areas for maximum energy output.

**Solar Irradiance Prediction and Rooftop Area Calculation Models**

This repository contains two machine-learning models: Solar Irradiance Prediction and Rooftop Area Calculation. The models are designed to work together to optimize solar panel installation and maximize solar energy output. The models utilize satellite images, machine learning algorithms, and image processing techniques.

**Solar Irradiance Prediction Model**

The Solar Irradiance Prediction model is implemented using a Long Short-Term Memory (LSTM) neural network architecture with the Keras library. The model predicts solar irradiance based on various features such as month, hour, latitude, longitude, panel capacity, panel efficiency, wind speed, cloud cover, and temperature. It is trained on a dataset that includes historical solar irradiance data and corresponding features. The model undergoes preprocessing steps including one-hot encoding of categorical features and scaling of numerical features. It is trained using the mean squared error (MSE) loss function and the Adam optimizer. Evaluation metrics such as MSE, RMSE, MAE, and R-squared are calculated for each month in the dataset. The model also provides the ability to predict irradiance for specific feature values.

**Rooftop Area Calculation and Solar Panel Fitment Model**

The Rooftop Area Calculation model utilizes the OpenCV library and image processing techniques to estimate the area of a rooftop from satellite images. In addition to calculating the rooftop area, the model is enhanced to determine the number of solar panels that can fit within that area. The image preprocessing steps involve converting the image to grayscale, applying histogram equalization to enhance contrast, and adaptive thresholding to separate the rooftop area from the background. The model removes the background from the original image using a binary mask generated from the preprocessing step. Contour analysis is performed on the binary mask to identify the roof contour. The contour with the largest area, which meets specific criteria such as minimum area and aspect ratio, is considered the rooftop contour. The area of the rooftop is calculated based on this contour. The model then estimates the number of solar panels that can fit within the calculated area based on predefined panel dimensions.

**Integration of Models**

The integration of the Solar Irradiance Prediction and Rooftop Area Calculation models allows for the optimization of solar panel installation and maximizing solar energy output. By combining the outputs of both models, users can assess the solar irradiance prediction for a given rooftop area and determine the maximum number of solar panels that can be installed within that area. This integration leverages satellite images and machine learning algorithms to provide accurate estimations and make informed decisions regarding solar energy planning. The integrated models offer opportunities for further customization and improvement based on specific requirements and datasets.

**Usage and Conclusion**

To utilize these models effectively, users need to provide relevant data, including satellite images and feature values for solar irradiance prediction. The models' parameters and thresholds can be adjusted based on specific needs and requirements. The integrated models provide valuable insights for solar energy planning, including predictions of solar irradiance and assessments of rooftop area and solar panel fitment. These insights can aid in optimizing solar panel installation and maximizing solar energy output. Further enhancements and customizations can be implemented to cater to unique use cases. The combination of satellite images, machine learning algorithms, and image processing techniques offers a powerful approach to solar energy planning and resource utilization.
