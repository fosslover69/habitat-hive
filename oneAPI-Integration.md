# Integrate oneAPI to your Project

This is a guide to Integrate oneAPI to your ML project.

To get started with oneAPI, Go to: https://devcloud.intel.com/oneapi/get_started/

Now you'll be granted with this page:
![image](https://user-images.githubusercontent.com/67329471/230723100-cfde23cc-9d28-4dad-a5ef-3f2989a4aa98.png)

Scroll down and click on Launch on Jupyter Lab (Assuming your code is on Jupyter Lab)
![image](https://user-images.githubusercontent.com/67329471/230723177-f8e7e687-9f58-4097-90b0-d4f48f42b9c6.png)

Now open the terminal by clicking on the Terminal Icon in Jupyter Lab
![image](https://user-images.githubusercontent.com/67329471/230723331-900d12f2-926b-4689-9f3e-af5af7fccdef.png)

Enter the following commands to install oneAPI kernel in your Jupyter Lab
```bash
mkdir MLoneAPI

cd MLoneAPI

source  /glob/development-tools/versions/oneapi/2022.3.1/inteloneapi/setvars.sh 

conda activate base

pip install ipykernel
python -m ipykernel install --user --name 2022.3.1 --display-name "oneAPI 2022.3.1"
```

Doing this will install oneAPI in your Jupyter Lab. After these procedures you can use oneAPI in your projects and enjoy your increased performance ; ). 
