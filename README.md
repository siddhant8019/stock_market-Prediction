## Program Details


1. Model Architecture Definition:
     - The code defines a Sequential model using TensorFlow's Keras API.
2. LSTM Layers with Dropout:
     - Four LSTM layers are added to the model, each followed by a dropout layer with a dropout rate 0.2 to prevent overfitting.
3. Input Shape:
     - The input shape for the first LSTM layer is specified as (X_train.shape[1], X_train.shape[2]) to match the shape of the input data.
4. Compilation:
     - The model is compiled with the Adam optimizer and sparse categorical cross-entropy loss function for multi-class classification.
5. Training and Evaluation:
     - The model is trained using the training data (x_train, y_train) with 5 epochs and a batch size 32.
     - Validation data (x_val, y_val) is used for validation during training.
     - After training, the model's performance is evaluated using the test data (x_test, y_test), and the test accuracy is printed.
