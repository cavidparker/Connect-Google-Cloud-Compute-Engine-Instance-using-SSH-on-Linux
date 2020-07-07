# Connect-Google-Cloud-Compute-Engine-Instance-using-SSH-on-Linux

### STEP 1 :
- (base) cavid@cavid-Z390-UD:~$ ssh-keygen -t rsa -f ~/.ssh/gcp -C "user_name"

### STEP 2 :
- (base) cavid@cavid-Z390-UD:~$ cd ~/.ssh

### STEP 3 :
- (base) cavid@cavid-Z390-UD:~/.ssh$ ls
- gcp(privet_key)  gcp.pub(public_key)  id_rsa  id_rsa.pub  known_hosts


### STEP 4 : 
- cat gcp.pub 

### STEP 5 :
- ssh -i gcp user_name@your_ip_address
- ssh -i gcp alien@35.2.0.0.0

## HOW TO RUN :
- GO To : cd ~/.ssh 
- ssh -i gcp alien@your_External IP

## HOW To Transfer file from computer to GCP :

- scp file_name yourhostname@Your_IP:your GCP directory(where you want to sent the file)

- scp image_resize.py alien@34.71.0.0.0:/home/alien

## Quickstart for Debian and Ubuntu :
- 1st step : Add the Cloud SDK distribution URI as a package source:
- echo "deb [signed-by=/usr/share/keyrings/cloud.google.gpg] http://packages.cloud.google.com/apt cloud-sdk main" | sudo tee -a /etc/apt/sources.list.d/google-cloud-sdk.list
- 2nd step : Import the Google Cloud Platform public key:
- curl https://packages.cloud.google.com/apt/doc/apt-key.gpg | sudo apt-key --keyring /usr/share/keyrings/cloud.google.gpg add -
- 3rd step: Update the package list and install the Cloud SDK
- sudo apt-get update && sudo apt-get install google-cloud-sdk
- ### LINK : https://cloud.google.com/sdk/docs/quickstart-debian-ubuntu

## Step:
- gcloud init
- gcloud app deploy app.yaml --project project_name


