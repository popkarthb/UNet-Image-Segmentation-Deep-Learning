##A description of the project
Built a 2 consecutive layers deep learning network model with UNet. Each consecutive layer include Conv2d + BatchNorm + ReLU layer. Down layers use Maxpool2d to downsample by a factor of 2. Up layers use Upsample to resize image.
Define and calculate loss function called DICE Loss Function. DICE is defined by two times Intersection of two input divided by the summation of the input.
Load the data into a PyTorch Dataset. Split the Dataset into training data and testing data. Load the data into torch data loader with a batch size of 8. And then feed the data into the model.
Run training epoch and setup model optimizer, monitor the training loss and validation loss. After 300 epochs, both losses drop under 0.1. Plot and shown the original image and segmentation image result.

##A description of the repository and code structure
HPML_FinalProject - Jupyter Notebook.pdf	---pdf version of HPML_FinalProject.ipynb
HPML_FinalProject.ipynb				---Main Program File
Image Segmentation via UNet.pdf			---project presentation
Loss.png					---Show how DICE cal
README.md					---This File.
UNET.png					---UNet architecture
UNet.drawio					---UNet architecture via drawio open with https://app.diagrams.net/
batch Data type.txt				---Show tensor datatype
conda_environment.yml				---File to creat enviroment in conda

##Example commands to execute the code         
conda env create -f conda_environment.yml
Example: https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html
Start up jupyter notebook with following command
jupyter notebook --ip 192.168.1.123 --port 8888
Open HPML_FinalProject.ipynb with your web browser
Run code with Jupyter Lab. Example: https://jupyter.org/

##Results (including charts/tables) and your observations  
See HPML_FinalProject - Jupyter Notebook.pdf