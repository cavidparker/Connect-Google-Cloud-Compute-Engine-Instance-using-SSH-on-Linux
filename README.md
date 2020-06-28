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

