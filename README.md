# HW5

#### Ansible Playbook:  


1. Install vagrant
2. Install virtual machine.
3. Setup 2 different vaitual machines using vagrant  
  (a) master server called ansible  
  (b) web server called node0  
4. Open 2 different terminals.
5. On each of the terminals start the vagrant machines using: vagrant ssh  
6. Use the .yml files with the terminal accessing the 'ansible' machine  
7. Run the following commands that execute the following tasks as follows:  

(a)  sudo ansible-playbook -i inventory setup.yml
  **Playbook for Setup: setup.yml **  
    
    * Installs node.js
    * Installs forever
    * Installs npm packages
    * Pull/clone git repo into a destination: https://github.com/CSC-DevOps/App
    
(b)  sudo ansible-playbook -i inventory tasks.yml
  **Playbook for Tasks: tasks.yml ** 

    * Runs app: `forever start main.js`
    * Ensures `bash`, `openssl`, `openssh-client`, and `openssh-server` are running latest version.
    * Removes content in `/tmp/*`

#### Concepts:  

    * Why should developers use configuration management tools to manage their software programs? What can go wrong?
    Answer:
    
    
    
    * Explain the difference bewteen continuous integration, continuous delivery, and continuous deployment, in your own words.
     Answer:
     Continuous Integration:
     For CI, for each new feature, bug fixes or improvement, one needs to write automated tests. Benefits: Obvious bugs are avoided being shipped to production. Building the release is easy.
     Continuous Delivery:
     For CD, Deployments need to be automated as in no manual involvement is required once it satrts. Benefits: No more complexity of deploying software. Release your product more often.
     Continuous Deployment:
     Benefits: Develop faster since no setbacks due to releases.Releases are less risky ans easier to fix. Contionuous stream of product improvement can be seen by the user.


#### [Screencast] (https://drive.google.com/open?id=1E78hTDLFTddvCyiPj-xLFfcgKOXcO1Jb)

  
 
