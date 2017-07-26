# auto-deploy

### Overview
With auto-deploy, Jupyter notebook can be deployed with their data onto Spark clusters in OpenShift without need to write Dockerfiles, manually create pods, or any of the other hassles that go with it. 

### Setup
Simply put all of your desired notebooks into a folder named `scripts`, your data into a folder named `data`, and then clone auto-deploy into the parent directory containing `scripts` and `data`. See [here](https://github.com/RobGeada/auto-deploy-template) for an example!

### Usage
Run `./auto-deploy -c [OPENSHIFT CLUSTER] -u [OS USERNAME] -p [OS PROJECT]` to get started. This command will generate an auto-deploy.config file, saving this configuration for later use via `./auto-deploy -f`. Check out `./auto-deploy -h` for more information.

The default password for the created Jupyter notebook server is **autodeploy**.
