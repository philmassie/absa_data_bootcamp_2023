# System setup and tooling
A critical step, and important to understand. Careful, here be dragons!
Even the simplest tooling up can eat up a lot of time, especially when exploring new toolsets and new OSs.
Our goal: Run some Python code in Jupyter notebooks.
Main tools: Anaconda, Jupyter, Git
1.	Anaconda
    - Widely used Python package and environment management, heavily marketed at data science community
    - Free and simple to use, at the expense of some bloat
    - we will use Anaconda to create a new python environment, install some packages, register a Jupyter kernel, launch Jupyter notebooks.
    - https://www.anaconda.com/download#downloads
2.	Git
    - Version control. We will use git to clone example files from GitHub
    - https://git-scm.com/download/win


## Install Anaconda
- Download the correct Anaconda for your OS from https://www.anaconda.com/download#downloads
- Double click the downloaded executable and follow the onscreen prompts:

![1](./images/Picture1.png)  
![1](./images/Picture2.png)  
![1](./images/Picture3.png)  
![1](./images/Picture4.png)  
![1](./images/Picture5.png)  
![1](./images/Picture6.png)  

### Setup a new Anaconda environment

- Run the **Anaconda Powershell Prompt**

![1](./images/Picture6a.png)  

- create a new environment and install a few packages to it using the Conda repositories
```
conda create -n data_bootcamp -y ipykernel pandas numpy scikit-learn seaborn
```
- Activate the environment. Once activated, running python in the powershell window will default to the eutable within the new environment.
- Create a new Jupyter kernel from the python environment. This allows Jupyter Notebooks to use the new Anaconda envi=ronment.

```
activate data_bootcamp2
python -m ipykernel install --user --name=data_bootcamp_kernel2
```

## Install Git
- Download the correct Git for your OS from https://git-scm.com/download
- Double click the downloaded executable and follow the onscreen prompts:
![1](./images/Picture7.png)  
![1](./images/Picture8.png)  
![1](./images/Picture9.png)  
![1](./images/Picture10.png)  
![1](./images/Picture11.png)  
![1](./images/Picture12.png)  
![1](./images/Picture13.png)  
![1](./images/Picture14.png)  
![1](./images/Picture15.png)  
![1](./images/Picture16.png)  
![1](./images/Picture17.png)  
![1](./images/Picture18.png)  
![1](./images/Picture19.png)  
![1](./images/Picture20.png)  
![1](./images/Picture21.png)  

## Clone this repo
Close and open the anaconda command prompt
change to your user directory, and clone this repo
```
c:
cd Users\yourusername
git config --global user.name "FIRST_NAME LAST_NAME"
git config --global user.email "MY_NAME@example.com"
git clone blah
```
