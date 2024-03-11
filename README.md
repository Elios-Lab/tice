# X
Embark on an exploration of the cutting-edge realm of Edge Intelligence with (X), an all-encompassing Deep Learning Notebook repository meticulously crafted for effortless implementation. Delve into five pivotal Jupyter Notebooks:

**X_Template**: The X Notebook consists of sections for deep learning for edge intelligences. The sections are as follows: Download Dataset, NN models, Linear Classifier, fully connected NN (MLP), CNN, Deeper CNN, tensorFlow Lite model, Post-training quantization, quantization aware training, and benchmark models with STM tools and boards.

   1. **Download Dataset**:
      * Allows users to insert dataset links and download them.
      * The notebook adeptly prepares and splits the dataset into training, validation, and testing datasets.
  2. **Linear Classifier (Baseline):**
     * Implements a linear SVM classifier with a grid of hyperparameter values.
     * Conducts a thorough hyperparameter study and selects the top three linear models.
     
  3. **Fully Connected NN (MLP):**
     * Implements a fully connected neural network.
     * Searches for optimal hyperparameter combinations, including hidden layers and units, ultimately choosing the three best MLP models.
  4. **CNN:**
     * Implements a CNN architecture with a Bayesian optimization algorithm.
     * Identifies the best hyperparameter combinations (learning rate, filters, dropout), creating and training three top-performing CNN models.
     * Concludes with an evaluation and visualization of each model's performance.
  5. **DCCN:**
     * Similar to the CNN section, enabling user choice of convolutional layers and kernel size.
  6. **TensorFlow Lite model:**
      * Converts the best models from each algorithm into TensorFlow Lite models.
      * Conducts an evaluation of TFLite models, ensuring seamless integration.
  7. **Post-quantization:**
      * Implements different quantization policies (dynamic, static, and full static) to convert models from float32 to 8-bit.
      * Evaluate quantized models for accuracy, model size, and precision.
  8. **Quantization Aware Training:**
      * Creates and trains quantization aware models (MLP, CNN, and DCNN).
      * Evaluate their performance, ensuring robust training and accurate results.
  9. **Benchmark Models with STM Tools:**
      * Installs STM libraries and selects boards for benchmarking.
      * Deploys the best models onto chosen boards, presenting comprehensive responses including ROM size, RAM size, weights size, and execution time.
    
**X_TOF**: Unleash the power of (X) with the X_TOF notebook, where the Time of Flight (TOF) dataset https://www.dropbox.com/s/4txj0ob6ovy9jbr/time-of-flight.zip?dl=1 takes center stage. This range imaging camera system measures distances based on time-of-flight, utilizing laser or LED signals. The notebook meticulously follows the X_Template steps—starting with dataset download, preparation, and preprocessing for training. A comprehensive hyperparameter study is conducted for each model, selecting the top three for further exploration. The notebook then transforms the best models into TFLite and performs quantization with various policies (Dynamic, Static, and Quantization aware training). Lastly, it installs STM libraries, selects STM boards, and analyzes the models on the chosen boards, providing insightful metrics on RAM, ROM, weights size, and Execution Time.

**X_EPD**: this notebook is similar to the X_TOF, where the analysis is conducted on electronics parts Imaging dataset (EPD). The dataset https://zenodo.org/records/6053169](https://github.com/praneelchand10/Electronics-Parts-Dataset.git  is composed of a total of 1734 images. Each class (capacitor, potentiometer, and regulator) had 578 images. The resolution of the camera is 30X30 pixels.

**X_SFD**: this notebook is similar to the X_TOF, where the analysis is conducted on Thermal Sign Language Imaging dataset (SFD). The dataset https://zenodo.org/records/6053169  contains low resolution thermal images corresponding to various sign language digits represented by hand and captured using the Omron D6T thermal camera. The resolution of the camera is 32X32 pixels.
Note: In X_SFD MobileNet is implemented since it`s support 32 by 32 images.
