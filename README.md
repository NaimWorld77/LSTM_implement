# Data Creation: 
Generated a sine wave sequence as synthetic time series data.
Prepared overlapping sub-sequences from the sine wave for training.
For each sequence, the next value was used as the target for prediction.

# Model Implementation: 
Built an LSTM model with:
1 LSTM layer to capture temporal dependencies.
1 fully connected layer (linear) to output the predicted next value.
ReLU activation for the LSTM layer.
Defined model input shape as (batch_size, seq_length, input_size) and output shape as (batch_size, 1).

# Training: 
Used Mean Squared Error (MSE) as the loss function for regression.
Applied Adam optimizer to minimize the loss function.
Trained the model over multiple epochs, printing the loss for monitoring.

# Model Evaluation: 
Evaluated the model in evaluation mode (model.eval()).
Compared predictions with actual values from test data.
Visualized predictions against ground truth using plots.

# Manual Testing: 
Provided custom input sequences (e.g., part of a sine wave).
Reshaped the input to match the model’s expected format.
Tested the model by passing the input and obtained a predicted next value.

# Final Outcome: 
The model was able to predict the next value in the sine wave sequence.
Manually tested input sequences confirmed that the model generalized well.
