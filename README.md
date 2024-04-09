
Introduction

This code provides functionality for preprocessing image datasets for machine learning tasks. It includes methods for data augmentation, resizing, balancing, splitting, normalization, encoding, dimensionality reduction, and handling skewed data. The primary aim is to prepare image data for training and testing machine learning models effectively.

Dependencies
Ensure you have the following dependencies installed:

* NumPy
* pandas
* OpenCV (cv2)
* imbalanced-learn (imblearn)
* scikit-learn (sklearn)
* Matplotlib

How to Use
1. Dataset Preparation: Organize your image dataset in a folder structure where each subfolder represents a class, and images belonging to that class are contained within.

2. Preprocessing: Use the provided functions to preprocess the dataset. You can perform various preprocessing steps such as data augmentation, resizing, balancing, normalization, encoding, dimensionality reduction, and handling skewed data. Ensure to adjust parameters as needed for your dataset.

3. Example Usage: The example provided demonstrates how to preprocess a dataset located at "Dataset(Augmented)/train". Modify the dataset_path variable to point to your dataset's location.

4. Label Mapping: Labels are converted to numerical values for model training. A label mapping is created to keep track of the mapping between class names and numerical labels.

5. Visualization: After preprocessing, you can visualize a few random images from each class to ensure data integrity and correctness. Adjust the number of images per class as needed.

6. Additional Notes: Ensure that your dataset contains a sufficient number of images for each class to prevent biased results.

Functions

* augment_data: Performs data augmentation on images.
* resize_images: Resizes images to a specified size.
* balance_data: Balances the dataset by oversampling minority classes.
* split_data: Splits the dataset into training and testing sets.
* normalize_data: Normalizes the data using min-max scaling.
* encode_categorical: Encodes categorical data using one-hot encoding.
* reduce_dimensionality: Reduces the dimensionality of data using PCA.
* handle_skewed_data: Applies log transformation to handle skewed data.
* load_and_preprocess_image: Loads and preprocesses images from file paths.
* preprocess_dataset: Preprocesses the entire dataset located in a specified path.

Contributions

Contributions are welcome! Feel free to fork this repository, make improvements, and submit pull requests.

License

This code is provided under the MIT License. See the LICENSE file for details.