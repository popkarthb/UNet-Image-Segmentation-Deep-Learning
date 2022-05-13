##A description of the project<br/>
Built a 2 consecutive layers deep learning network model with UNet. Each consecutive layer include Conv2d + BatchNorm + ReLU layer. Down layers use Maxpool2d to downsample by a factor of 2. Up layers use Upsample to resize image.
Define and calculate loss function called DICE Loss Function. DICE is defined by two times Intersection of two input divided by the summation of the input.
Load the data into a PyTorch Dataset. Split the Dataset into training data and testing data. Load the data into torch data loader with a batch size of 8. And then feed the data into the model.
Run training epoch and setup model optimizer, monitor the training loss and validation loss. After 300 epochs, both losses drop under 0.1. Plot and shown the original image and segmentation image result.

##A description of the repository and code structure<br/>
HPML_FinalProject - Jupyter Notebook.pdf	---pdf version of HPML_FinalProject.ipynb<br/>
HPML_FinalProject.ipynb				---Main Program File<br/>
Image Segmentation via UNet.pdf			---project presentation<br/>
Loss.png					---Show how DICE cal<br/>
README.md					---This File.<br/>
UNET.png					---UNet architecture<br/>
UNet.drawio					---UNet architecture via drawio open with https://app.diagrams.net/<br/>
batch Data type.txt				---Show tensor datatype<br/>
conda_environment.yml				---File to creat enviroment in conda<br/>

##Example commands to execute the code<br/>
conda env create -f conda_environment.yml<br/>
Example: https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html<br/>
Start up jupyter notebook with following command<br/>
jupyter notebook --ip 192.168.1.123 --port 8888<br/>
Open HPML_FinalProject.ipynb with your web browser<br/>
Run code with Jupyter Lab. Example: https://jupyter.org/

##Results (including charts/tables) and your observations<br/> 
See HPML_FinalProject - Jupyter Notebook.pdf