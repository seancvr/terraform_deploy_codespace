FROM mcr.microsoft.com/devcontainers/base:noble

RUN sudo apt update && sudo apt upgrade -y

#-----Terraform installation commands-----
# Install gnupg and software-common-properties packages
RUN sudo apt-get install -y gnupg software-properties-common

# Install HashiCorp GPG key
RUN wget -O- https://apt.releases.hashicorp.com/gpg | \
    gpg --dearmor | \
    sudo tee /usr/share/keyrings/hashicorp-archive-keyring.gpg > /dev/null

# Add HashiCorp repo to your system
RUN echo "deb [signed-by=/usr/share/keyrings/hashicorp-archive-keyring.gpg] \
    https://apt.releases.hashicorp.com $(lsb_release -cs) main" | \
    sudo tee /etc/apt/sources.list.d/hashicorp.list

# Download package info from HashiCorp
RUN sudo apt update

# Install Terraform from the new repo
RUN sudo apt install -y terraform
