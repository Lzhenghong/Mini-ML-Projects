Summary:
Image classification using Transfer Learning by fine-tuning EfficientNetB0 model and mixed precision

Dataset:
food101 TensorFlow dataset

Description:
- Load images and labels from food101
- Conduct train-test split on dataset
- Create a mapping function to resize images into 224x224 and convert into tensors of type float32
- Apply mapping function to images and turn them into batches of size 32
- Optimise data preprocessing using parallelisation
- Activate mixed precision
- Build a feature extraction model from EfficientNetB0
- Fine tune the model by unfreezing all layers
- Fit the train dataset to fine-tuned model and validate using test dataset

Results:
- 96.7% training accuracy
- 77.8% validation accuracy
