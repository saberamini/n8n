# Create an EC2 instance
- Create an EC2 instance in AWS 
- Use Ubuntu as the operating system
- Have 32 G of space
- Use t2.medium

# Create Security Group
- Create a security group that allows traffice on port 22 (SSH) and port 5678 (n8n server)
- attach security group to the EC2 instance

# Install approproach packages
- go to the home directory by typing 
<pre><code>bash cd ~ </code></pre>

- open the .bashrc file
<pre><code>nano .bashrc</code></pre>

- At the buttom of the file, type the following
 <pre><code>export N8N_SECURE_COOKIE=false</code></pre>
- update packages by running folowing command 
 <pre><code>sudo apt update</code></pre>

- install node package manager
<pre><code>sudo apt install npm</code></pre>
# Start n8n Server
- install and run server with following command
<pre><code>npx n8n</code></pre>
