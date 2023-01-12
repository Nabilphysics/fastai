## fastai installation on Ubuntu using miniconda
### Step 1: Install Miniconda
```
sudo apt update && sudo apt upgrade
```
```
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
```
```
bash Miniconda3-latest-Linux-x86_64.sh
```
Hit the Enter key to start the installation process. Soon, the installer will ask to accept the License, press q, and then type Yes to accept it. The setup will also you – “Do you wish the installer to initialize Miniconda3 by running Conda init?” If you type Yes then every time you open the Terminal, Conda’s base environment will be activated on startup and also this will add the Conda3 folder path in your bash profile. Hence, it is recommended to type –Yes. 

Tips: In case you have activated the base environment of Condo to start every time with terminal and now you want to deactivate it, then here is the command to follow:
```
conda config --set auto_activate_base false
```
### Step 2: Create, Activate or Deactivate Virtual Environment
Create: 
```
conda create -n [environment-name] -y
```
Activate: 
```
conda activate [environment-name]
```
Deactivate:
```
conda deactivate
```
Useful Blog about Conda: https://www.how2shout.com/linux/install-miniconda-on-ubuntu-22-04-lts-jammy-linux/ and https://faisalmalikwp.medium.com/install-and-configure-jupyter-lab-using-miniconda-on-ubuntu-18-04-b7abd3f411a8
### Step 3: Install Fastai
```
conda install -c fastchan fastai
```
Official Link: https://docs.fast.ai/

### Step 4: Install and Start Jupyter Notebook
To install
```
conda install jupyterlab -y
```
To start:
```
jupyter notebook
```


