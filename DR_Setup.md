<h1>AWS Disaster Recovery Plan Setup </h1>

<h2>CRUD</h2>

- Create
- Read 
- Update 
- Delete

![AWSCLI diagram](https://user-images.githubusercontent.com/126012715/234847404-800d0f1e-c2c5-4188-8246-40fdc6a711f3.JPG)

<h3>Pre-requisites</h3>

- Must have access key and secrey keys
- Move the keys to your .ssh folder 
- SSH your ec2 instance into the same region in the terminal and use ubuntu 18.04
- Setup of AWS CLI (command line interface)
- Applying CRUD from the AWSCLI from the ec2 instance


<h3>Getting everything setup</h3>

<h4>Step 1</h4>

- Run the following commands once connected to ec2 instance in the terminal.

`sudo apt update -y`

`sudo apt upgrade -y`

`python3 --version`

<h4>Step 2</h4>

Installing python and latest pip version on Linux

`sudo apt-get install python3.9` , latest version of python

You may use your `sudo nano .bashrc` to edit the alias and enter `alias python=python3` or

`alias python=python3`

<h4>Step 3</h4>

Then install python onto the ec2 instance

`sudo apt install python`

Then install pip

`sudo apt-get install python3-pip`

Install AWSCLI and boto3 

`sudo python3 -m pip install awscli` or

`sudo pip3 install awscli`

`sudo pip3 install boto3`

<h4>Step 4</h4>

Connect to the AWS through terminal.

Run `aws configure` and follow the instructions.

- Copy and paste the access key ID and the secret key when prompted 
- Default region = `[eu-west-1]`
- Output format = `json`
- Validates and show's the content within s3 container `aws s3 ls` if error, re-do the steps from `aws configure`










