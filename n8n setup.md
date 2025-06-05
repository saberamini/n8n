# Create an EC2 instance
- Create an EC2 instance in AWS 
- Use Ubuntu as the operating system
- Have 32 G of space
- Use t2.medium

# Create Security Group
- Create a security group that allows traffice on port 22 (SSH) and port 5678 (n8n server)
- attach security group to the EC2 instance

# Install approproach packages
- go to the home directory by typing `cd ~
- open the .bashrc file `nano .bashrc
- At the buttom of the file, type the following
` export N8N_SECURE_COOKIE=false
- update packages by running folowing command `sudo apt update
- install node package manager `sudo apt install npm

# Start n8n Server
- install and run server with following command
`npx n8n