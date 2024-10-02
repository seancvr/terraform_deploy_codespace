# Terraform deployment codespace
This repository contains the instructions for creating a custom codespace for deploying resources to the cloud with Terraform. 
Currently it's just configured with Azure cli, but it can be customized to integrate with other cloud providers.    

It contains the following tools:

- Azure cli
- Terraform
- git
- wget
- curl

The tooling for this container can be customized in the devcontainer.json and Dockerfile files. 
## Creating a codespace

With the Visual Studio Code "Remote Explorer" icon selected, 
<p align="left">
  <img src="pictures/remote_explorer_icon.png" width="10%" height="15%" title="remote_explorer">
</p>

click the "Create Codespace" button.
<p align="left">
  <img src="pictures/create_codespace.png" width="40%" height="30%" title="create_codespace">
</p>

Select the repo with the devcontainer.json and Dockerfile that specifies your desired container.
<p align="left">
  <img src="pictures/select_repo.png" width="40%" height="30%" title="select_repo">
</p>

Select the repository branch, in this case the main branch. 
<p align="left">
  <img src="pictures/default_branch.png" width="40%" height="30%" title="create_new_cs">
</p>

Select the resources you would like to allocate to your codespace.
<p align="left">
  <img src="pictures/codespace_resources.png" width="40%" height="30%" title="codespace_resources">
</p>

After that your codespace window will open, with a progress bar at the bottom right showing the build status. 
<p align="left">
  <img src="pictures/building_codespace.png" width="40%" height="30%" title="building_codespace">
</p>
