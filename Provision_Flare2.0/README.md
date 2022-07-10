# PROVISION TOOL IN FLARE 2.0

A necessary first step in establishing a federation is provisioning to establish the identities of the server, clients, and admin clients. 

The below diagram describes the architecture of NVIDIA FLARE Open Provision API in blue. Those two green blocks are the sample python code (provision.py) collecting project configuration information (project.yml) and interacting with components of Open Provision API to accomplish a provisioning task. The Provisioner and blocks inside the blue box are classes or subclasses of Open Provision API. 

For more details, refer to the official documentation. 

<p align="center">
  <img src="https://github.com/ajulyav/NVIDIA_FLARE/blob/main/Provision_Flare2.0/imgs/1.png" width="650">
</p>

If one wants to test a Federation not in POC environment, but in real-world mode, call the Provision tool graphic interface tool. To do so, in the virtual (or conda) enviroment with the installed nvflare package: 

```
provision -u
```
If successful, the start page of the Provision tool is snown. Here are some examples:
<p align="center">
  <img src="https://github.com/ajulyav/NVIDIA_FLARE/blob/main/Provision_Flare2.0/imgs/2.png" width="450">
  <img src="https://github.com/ajulyav/NVIDIA_FLARE/blob/main/Provision_Flare2.0/imgs/3.png" width="450">
  <img src="https://github.com/ajulyav/NVIDIA_FLARE/blob/main/Provision_Flare2.0/imgs/4.png" width="450">
</p>
