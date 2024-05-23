# Requirements
Make sure that you have the following installed:
- [node](https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-ubuntu-18-04) 
- npm 
- [MongoDB](https://docs.mongodb.com/manual/tutorial/install-mongodb-on-ubuntu/) and start the mongodb service with `sudo service mongod start`

## Navigate to the Client Folder 
 `cd client`

## Run the folllowing command to install the dependencies 
 `npm install`

## Run the folllowing to start the app
 `npm start`

## Open a new terminal and run the same commands in the backend folder
 `cd ../backend`

 `npm install`

 `npm start`

 ### Go ahead a nd add a product (note that the price field only takes a numeric input)

 # Docker Compose
 1. Clone the repository

 2. Ensure that you have docker installed

 ## To run all the services at once you can use 
     `docker-compose up`
     
   All the containers will be up and running

 ##   To access the fronted 
     'http://localhost:3000/' 
   Use this link to access the fronted.
  ## sample fronted image

   ![alt text](image-2.png)


## Running with Ansible

If you have Ansible installed, you can use it to automate the deployment of the application. Here's a basic example of how you might do this:

1. First, install Ansible , Vagrant, Virtual Box and terraform on your local machine. You can do this with the following command:

```bash
sudo apt-get update
sudo apt-get install ansible vagrant virtualbox
```


2. Run the playbook with the following command:
  
```bash
vagrant up 
```
3. To run with terraform :
```bash
terraform init
terraform plan 
```
