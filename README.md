# UNet-Image-Segmentation-Deep-Learning

•	Built a 2 consecutive layers deep learning network model with UNet. Each consecutive layer include Conv2d + BatchNorm + ReLU layer. Down layers use Maxpool2d to downsample by a factor of 2. Up layers use Upsample to resize image.

•	Define and calculate loss function called DICE Loss Function. DICE is defined by two times Intersection of two input divided by the summation of the input.

•	Load the data into a PyTorch Dataset. Split the Dataset into training data and testing data. Load the data into torch data loader with a batch size of 8. And then feed the data into the model.

•	Run training epoch and setup model optimizer, monitor the training loss and validation loss. After 300 epochs, both losses drop under 0.1

•	Correct plot and shown the original image and segmentation image result.
