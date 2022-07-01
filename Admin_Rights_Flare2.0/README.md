# Rights and Permissions 

Nvidia Provision tool provides the possibility to grant certain rights to the participants of a FL experiment.


All available rights in versions prior to 2.1 are shown in the image below. For instance:
1. "Upload App" allows a member to upload a custom folder (i.e. code, user/server configurations) to the Server (to the Transfer folder)
2. "Deploy All/Self" allows a member to send a custom folder to all/some experiment participants.
3. "Train All/Self" allows a member to start an experiment on all/some participant sides.
4. "View All/Self" allows a member to see certain information about all/some paricipants (i.e. workstations, Server).
5. "Operate All/Self" allows a member to abort/restart and etc. all/some participants (i.e. workstations, Server).

<p align="center">
  <img src="https://github.com/ajulyav/NVIDIA_FLARE/blob/main/Admin_Rights_Flare2.0/imgs/1.png" width="750">
</p>

As it can be seen, some rights are devided into "All" and "Self". The diagrams below show the main difference between these two types. For a visual explanation, imagine a simple structure where there is:
- two organizations: Organization 1 and Organization 2;
- Organization 1 has: Server, Super Admin with all Super rights (marked as "All" where it is possible), as well as a Regular User (without access to any admin console);
- Organization 2 has: 3 workstations, in particular, on the 1st station there is a Regular User (no admin console) and a Researcher (only has the right to "Upload App" to the Server), on the 2nd station - a Regular User (no admin console), on the 3rd - again a Regular User and a Local Admin with a set of rights ("View Self", "Operate Self", "Upload App", "Deploy Self", "Train Self").



<p align="center">
  <img src="https://github.com/ajulyav/NVIDIA_FLARE/blob/main/Admin_Rights_Flare2.0/imgs/2.png" width="500">
  <img src="https://github.com/ajulyav/NVIDIA_FLARE/blob/main/Admin_Rights_Flare2.0/imgs/3.png" width="500">
</p>


1. "View Self": So, from Organization 2, one can see only sites (workstations) of Organization 2, but not of Organization 1. Also, one cannot see the Server too if this is in Organization 1. <br />
  "View All": (Super Admin): can see all sites and all Organizations. 
  
2. "Operate Self": From Organization 2, one cannot restart/stop... the Server in Organization 1 (even when knowing the username & password of Super Admin). <br />
  "Operate All": I.e. Super Admin can stop/restart... any sites in any Organization.


<p align="center">
  <img src="https://github.com/ajulyav/NVIDIA_FLARE/blob/main/Admin_Rights_Flare2.0/imgs/4.png" width="500">
  <img src="https://github.com/ajulyav/NVIDIA_FLARE/blob/main/Admin_Rights_Flare2.0/imgs/5.png" width="500">
</p>

3. "Upload App": Local Admin in Organization 2 can send custom code/config files from the local Transfer folder to the Server (to the Transfer folder)
4. "Deploy Self":  Local Admin in Organization 2 can deploy an app (send custom code and config files) to any/all sites within Organization 2, but not outside of it. <br />
    "Deploy All": Super Admin can deploy an app to any clients or choose a particular one (as a cohort) by providing names.


<p align="center">
  <img src="https://github.com/ajulyav/NVIDIA_FLARE/blob/main/Admin_Rights_Flare2.0/imgs/6.png" width="500">
</p>

5. "Train Self":  Local Admin in Organization 2 can start an experiment (i.e. training or validation) on any/all sites within Organization 2, but not outside of it. <br />
    "Train All": Super Admin can start an experiment on any clients or choose a particular one (as a cohort) by providing names.
