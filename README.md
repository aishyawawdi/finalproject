# Final project 
currency changer are common features in AI applications.
In the following assignment we are implemented a web server that handles
calculation of currency change. For example, given an amount in one currency we would like to calculate that amount in 
another currency etc
you can by click **Auti** butten see all the change history 

## Common setup
Clone the repo and install the dependencies.
```bash
git clone https://github.com/mohamaddiwany/finalproject.git
```

## Usage - By Flask

open Command Prompt and go to the file location then tap 
```bash
py -m pip install -r requirements.txt
set FLASK_APP=main.py
flask run
```
Go over the [localhost](https://127.0.0.0:5000) with port 5000 because flask run with that port

## Usage - By Docker

open Command Prompt and go to the file location then tap
```bash
docker build -t frontend .
```
that's will build the docker image for you then tap
notice: a docker demon must be running before building the image
```bash
docker run -d -p 5000:5000 frontend
```
Go over the [localhost](https://127.0.0.0:5000)

## Usage - kubernetes:  
```bash
git clone https://github.com/mohamaddiwany/finalproject.git
cd finalproject
cd k8s  
kubectl apply -f backend.yml -f frontend-.yml -f auti.yml  
```

open your browser and go to [localhost](https://127.0.0.0:31495) "127.0.0.1:31495"  

## Usage - By Terraform:  
```bash
git clone https://github.com/mohamaddiwany/finalproject.git  
cd finalproject  
```
go to main.tf file  
change the key name your Keypair name in your aws   
add your privte key file to the folder (something which end with .pem)
set your access_key and secret_key of aws instead of #####
then work like we used to work on terraform

terraform init - to start the work 
terraform apply - to make it run 

not to forget then to destroy the terraform:  
terraform destroy
  
then go to your aws console and get your instance public ip run through "your-instance-ip:5002"  


