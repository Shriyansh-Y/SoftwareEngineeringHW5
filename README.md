# HW5

#### Ansible Playbook:  


1. Install vagrant
2. Install virtual machine.
3. Setup 2 different virtual machines using vagrant  
  (a) master server called ansible  
  (b) web server called node0  
4. Open 2 different terminals.
5. On each of the terminals start the vagrant machines using: vagrant ssh  
6. Use the .yml files with the terminal accessing the 'ansible' machine  

7. Run the following commands that execute the following tasks as follows:  

(a)  sudo ansible-playbook -i inventory setup.yml  

    * Installs nodejs
    * Installs forever
    * Installs npm packages
    * Pull/clone git repo into a destination: https://github.com/CSC-DevOps/App  
    
(b)  sudo ansible-playbook -i inventory tasks.yml

    * Runs app: `forever start main.js  <port number>``
    * Ensures `bash`, `openssl`, `openssh-client`, and `openssh-server` are running latest version.
    * Removes content in `/tmp/*`

#### Concepts:  

You can see the solutions to the questions in [Solutions](https://github.ncsu.edu/scyadav/HW5/blob/master/Solutions.pdf)


#### Screencasts:


* Only execution of playbooks and verification: [Screencast for running ansible playbooks](https://youtu.be/bSa4i8uZIZw)  
 
* In case one needs to see the complete setup from installing vagrant commands to running playbook: [Complete Setup, tasks, running playbook](https://youtu.be/6lW9FYo6Zpk)  


  
 
