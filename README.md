# Machine Learning Projects

<details>
<summary><h3>CNN - Image Classification with the Mars Curiosity Rover</h3></summary>
This project focused on classifying images taken by the Curiosity Mars Rover into one of 25 distinct categaroies using a Convolutional Neural Network (CNN). After this, the model was changed to perform binary classification and categorise the images based on if they contained a part of the rover or not.
<br/><br/>

- Utilised `ImageDataGenerator` to load and rescale the image data, and prepared batches for training while also exploring and pre-processing the dataset.
- Implemented a CNN model (using TensorFlow and Keras libraries to perform the classification task) to train on 3746 images and experimented with the network architecture for this particular problem.
- Optimised hyperparameters such as batch size and dropout to improve accuracy while reducing runtime.
- Evaluated the initial model's performance with accuracy and loss plots, and a histogram showing the distribution of Correct vs Incorrect predictions per class.
<br/><br/>

<img src = "Plots/CNN - Mars Rover/25_images.png">
<img src = "Plots/CNN - Mars Rover/histogram.png">
<img src = "Plots/CNN - Mars Rover/accuracy.png">
<img src = "Plots/CNN - Mars Rover/roc_curve.png">
</details>

<details>
<summary><h3>CNN - Image Classification from a Kaggle-sourced anime dataset</h3></summary>

| Data | Link |
| --- | --- |
| Original dataset | [Kaggle](https://www.kaggle.com/datasets/diraizel/anime-images-dataset) |
| Modified dataset (Used in this project) | [Google Drive](https://drive.google.com/file/d/1B9xa70mfSjKxEO_OKrbuQlPtdIj1wlDL/view?usp=sharing) |

<!---
Dataset obtained from https://www.kaggle.com/datasets/diraizel/anime-images-dataset

Access modified dataset used below from https://drive.google.com/file/d/1B9xa70mfSjKxEO_OKrbuQlPtdIj1wlDL/view?usp=sharing
-->

[original dataset]: <> (Dataset obtained from https://www.kaggle.com/datasets/diraizel/anime-images-dataset)
[modified dataset]: <> (Access modified dataset used below from https://drive.google.com/file/d/1B9xa70mfSjKxEO_OKrbuQlPtdIj1wlDL/view?usp=sharing)

This project also classified images; however, these images were from a subset of popular anime titles in a Kaggle dataset. For training, validation and testing, 6573, 1618 and 2040 images were used, respectively; this was a collection of approximately 300 images representing each of the 28 chosen classes.
<br/><br/>

- Developed and trained a CNN to perform classification, labelling each of the training images with a predicted class from the 28 available.
- Combined part of the image pre-processing into the CNN with a lamda layer in between the input and first convolutional layers, resizing each image as it is put into the network.
- Experimented with the network architecture and hyperparameters to result in a CNN optimised for this dataset and task.
- Evaluated the model's performance through a combination of:
  - Accuracy and Loss plots
  - Histograms of the Correct vs. Incorrect label predictions per class
  - Line graphs of the model's percentage accuracy for each class
  - Confusion matrices
<br/><br/>

<img src = "Plots/CNN - Anime/CNN_images.png">
<img src = "Plots/CNN - Anime/CNN_hist_acc.png">
<img src = "Plots/CNN - Anime/CNN_confusion.png">
</details>

<details>
<summary><h3>MLP - Prediction of z-band brightness of quasars, given the brightness in i- and r-bands</h3></summary>
This project used machine learning to predict a quasar's brightness in the z-band after training a Multi-Layer Perceptron (MLP) on the quasar's brightness in the i- and r-bands.
<br/><br/>

- Created a heatmap of the dataset to visualise correlations between different variables, choosing the optimal set to perform multi-variable regression with.
- Developed and trained an MLP on the selected data after pre-processing, allowing the network to take in the i- and r-band magnitudes.
- Tuned hyperparameters like batch size, learning rate, dropout and hidden layers to optimise the network performance.
- Evaluated the model using Mean Squared Error (MSE), achieving an MSE loss of 0.072, and residual analysis on the test data.
<br/><br/>

<img src = "Plots/MLP - Quasars/MLP_imag_prediction.png">
<img src = "Plots/MLP - Quasars/MLP_rmag_prediction.png">
<img src = "Plots/MLP - Quasars/MLP_imag_rmag_residuals.png">
</details>
