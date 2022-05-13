##A description of the project
__Built a 2 consecutive layers deep learning network model with UNet. Each consecutive layer include Conv2d + BatchNorm + ReLU layer. Down layers use Maxpool2d to downsample by a factor of 2. Up layers use Upsample to resize image.
Define and calculate loss function called DICE Loss Function. DICE is defined by two times Intersection of two input divided by the summation of the input.
Load the data into a PyTorch Dataset. Split the Dataset into training data and testing data. Load the data into torch data loader with a batch size of 8. And then feed the data into the model.
Run training epoch and setup model optimizer, monitor the training loss and validation loss. After 300 epochs, both losses drop under 0.1. Plot and shown the original image and segmentation image result.

##A description of the repository and code structure
__HPML_FinalProject - Jupyter Notebook.pdf	---pdf version of HPML_FinalProject.ipynb
__HPML_FinalProject.ipynb				---Main Program File
__Image Segmentation via UNet.pdf			---project presentation
__Loss.png					---Show how DICE cal
__README.md					---This File.
__UNET.png					---UNet architecture
__UNet.drawio					---UNet architecture via drawio open with https://app.diagrams.net/
__batch Data type.txt				---Show tensor datatype
__conda_environment.yml				---File to creat enviroment in conda

##Example commands to execute the code         
__conda env create -f conda_environment.yml
__Example: https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html
__Start up jupyter notebook with following command
__jupyter notebook --ip 192.168.1.123 --port 8888
__Open HPML_FinalProject.ipynb with your web browser
__Run code with Jupyter Lab. Example: https://jupyter.org/

##Results (including charts/tables) and your observations  
__See HPML_FinalProject - Jupyter Notebook.pdf