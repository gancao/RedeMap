# RedeMap #

![RedeMap](https://github.com/gancao/RedeMap/blob/main/Figure1.png)

## Web ##
We provided a web program bulit by Django for visualizing the the distribution of any intersested cell states that express user-defined gene sets across various healthy or primary tumor tissues as well as other correlation analysis.
We also provided windows and linux versions for all users.

![RedeMap](https://github.com/gancao/RedeMap/blob/main/RedeMap.png)

## Download ##
    First, you should download the program files from the below wensite:
    https://zenodo.org/records/17509468
    Then, you should unzip the corresponding files in a directory. If you want to run RedeMap on a windows system, please use "RedeMap_win.zip". If you want to run RedeMap on a linux system, please use "RedeMap_linux.zip".

## Usage ##
Before running RedeMap, the users should finish the following steps to use this web tool. <br>

**step1: Install R4 and Python3 on your computer and save the installed paths into the environment variables** <br>

**step2: Install required R and python packages** <br>

    pip install -r requirements.txt
    R path/Rscript install_r_packages.R

**step3: Define the path of R in ImmunoMap/views.py** <br>

    os.environ['PATH'] = r"D:\Program Files (x86)\R-4.2.2\bin;" + os.environ['PATH']
    #or
    os.environ['PATH'] = "/home/software/miniconda3/envs/R4/bin;" + os.environ['PATH']

**step4: Run RedeMap using 8000 port** <br>

    python manage.py runserver 0.0.0.0:8000    

**step5: Open RedeMap in the browser** <br>

    #if you have successfully run RedeMap on your own windows computer, the website can be visited by:
    http://127.0.0.1:8000/ImmunoMap/    
    #if you have successfully run RedeMap on the linux system, the website can also be visited on your own windows computer by:
    http://linux IP:8000/ImmunoMap/
