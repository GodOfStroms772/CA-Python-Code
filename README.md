# CA-Python-Code
Instructions

You need to run the python script through the Google Cloud SDK Shell terminal and it will create a virtual machine with all the given parameters.
To run the script, execute:
py pycode.py


Prerequisites 

You need to have the Google Cloud SDK Shell installed on your machine and then create a project. From within GCE you need to add Identity and Access Management permissions.
As well as setting up your system to allow APIs to be called. 
Ensure you excecute the following lines:

pip install google-api-python-client google-auth google-auth-httplib2 google-auth-oauthlib oauth2client

gcloud auth application-default login

gcloud auth application-default set-quota-project hardy-pattern-456119-p6


Output and Troubleshooting

If the python script successfully creates the VM instance the following will be output:
Checking if static IP already exists...
Static IP not found. Creating a new one...
Checking if firewall rule already exists...
Firewall rule 'allow-http-ssh' not found. Creating it...
Creating VM instance...
Waiting for instance to be ready...
Instance created.

For the troubeshooting you need to make sure the static ip or firewall has already been created and handle this scenario accordingly. If successful the following will be output:
Checking if static IP already exists...
Static IP already exists. Reusing it.
Checking if firewall rule already exists...
Firewall rule 'allow-http-ssh' already exists. Skipping creation.
Creating VM instance...
Waiting for instance to be ready...
Instance created.