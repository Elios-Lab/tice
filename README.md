# TICE - Tiny Image Classification Explorer
Embark on an exploration of the cutting-edge realm of Edge Intelligence with TICE, an all-encompassing Deep Learning Notebook repository meticulously crafted for effortless implementation. Delve into five pivotal Jupyter Notebooks:

**Template**: The TICE Notebook consists of sections for deep learning for edge intelligence. The sections are as follows:

   1. **Download Dataset**:
      * Allows users to insert dataset links and download them.
      * The notebook adeptly prepares and splits the dataset into training, validation, and testing datasets.
      * It also visualizes some images of the dataset, ensuring a comprehensive understanding of the data.
   2. **NN Models**:
      * Implements the functions to be used for DL studies.
      * The notebook includes functions for training, evaluating, and visualizing the performance of the models.

   3. **Linear Classifier (Baseline)**:
      * Implements a linear SVM classifier with a grid of hyperparameter values.
      * Conducts a thorough hyperparameter study and selects the top three linear models.

   4. **Decision Tree (Random Forest Classifier)**:
      * Implements a Random Forest Classifier with a grid of hyperparameter values.
      * Conducts a thorough hyperparameter study and selects the top three linear models.

   5. **KNN Classifier**:
      * Implements a KNN Classifier with a grid of hyperparameter values.
      * Conducts a thorough hyperparameter study and selects the top three linear models.
     
   6. **Fully Connected NN (MLP):**
      * Implements a fully connected neural network.
      * Searches for optimal hyperparameter combinations, including hidden layers and units, ultimately choosing the three best MLP models.

   7. **CNN:**
      * Implements a CNN architecture with a Bayesian optimization algorithm.
      * Identifies the best hyperparameter combinations (learning rate, filters, dropout), creating and training three top-performing CNN models.
      * Concludes with an evaluation and visualization of each model's performance.

   8. **DCCN:**
      * Similar to the CNN section, enabling user choice of convolutional layers and kernel size.

   9. **TensorFlow Lite model:**
      * Converts the best models from each algorithm into TensorFlow Lite models.
      * Conducts an evaluation of TFLite models, ensuring seamless integration.

   10. **Post-training quantization:**
      * Implements different quantization policies (dynamic, static, and full static) to convert models from float32 to 8-bit.
      * Evaluate quantized models for accuracy, model size, and precision.

   11. **Quantization Aware Training:**
      * Creates and trains quantization aware models (MLP, CNN, and DCNN).
      * Evaluate their performance, ensuring robust training and accurate results.

   12. **Benchmark Models with STM tools:**
      * Installs STM libraries and selects boards for benchmarking.

   13. **Benchmark Models on STM boards:**
      * Deploys the best models onto chosen boards, presenting comprehensive responses including ROM size, RAM size, weights size, and execution time.

   14. **Generate C Code:**
      * Generates C code for the best models, ensuring seamless integration with STM boards.
    
**TOF**: The [Time of Flight (TOF) dataset](https://www.dropbox.com/s/4txj0ob6ovy9jbr/time-of-flight.zip?dl=1) takes center stage. This range imaging camera system measures distances based on time-of-flight, utilizing laser or LED signals. The images size is 8x8. The notebook meticulously follows the X_Template steps—starting with dataset download, preparation, and preprocessing for training. A comprehensive hyperparameter study is conducted for each model, selecting the top three for further exploration. The notebook then transforms the best models into TFLite and performs quantization with various policies (Dynamic, Static, and Quantization aware training). Lastly, it installs STM libraries, selects STM boards, and analyzes the models on the chosen boards, providing insightful metrics on RAM, ROM, weights size, and Execution Time.

**EPD**: This notebook is similar to the TOF, where the analysis is conducted on [electronics parts Imaging dataset (EPD)](https://github.com/praneelchand10/Electronics-Parts-Dataset.git). The dataset is composed of a total of 1734 images. Each class (capacitor, potentiometer, and regulator) had 578 images. The resolution of the camera is 30x30 pixels.

**ITD**: A low-resolution [infrared thermal dataset (ITD)](https://zenodo.org/records/5574233/files/Infrared%20thermal%20dataset.zip) of people and thermal objects, such as a working laptop, in indoor environments. The dataset was collected by a far infrared thermal camera (32x24 pixels), which can capture the position and shape information of thermal objects without privacy issues that enable trustworthy computer vision applications. The dataset consists of 1770 thermal images with high-quality annotation collected from an indoor room with around 15°C.

**SFD**: In this notebook, the analysis is conducted on the [Sign Finger Digits (SFD) dataset](https://zenodo.org/records/6053169). The dataset contains low resolution thermal images corresponding to various sign language digits represented by hand and captured using the Omron D6T thermal camera. The resolution of the camera is 32x32 pixels.
Note: In X_SFD MobileNet is also implemented since it supports 32x32 images.

## Publication
This work has been published in [IEEE Open Journal of the Industrial Electronics Society](https://doi.org/10.1109/OJIES.2024.3451959).

Please cite the paper if you use this code.
