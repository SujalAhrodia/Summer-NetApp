<img src="https://raw.githubusercontent.com/SujalAhrodia/Summer-NetApp/master/Resources/NetAppLogo.png" width="300"> 

# Summer-Internship 

## Structure

> * main.yml contains the basic ONTAP Lab
> * All the express guide playbooks are in the Express-Guides folder

## 1. Setting up the environment
  * Cluster with an HA pair running ONTAP 9.5
  * Jumphost, CentOS-7-x86_64-Minimal-1810
## 2. On the jumphost:
  * Clone the repo
    ```shell
    $ git clone https://github.com/SujalAhrodia/Summer-NetApp.git
    ```  
  * Install the latest version of ansible(atleast 2.6)
    ```shell
    $ yum install ansible
    ```
  <!-- * Install pip for python2 
    ```shell
    $ sudo apt install python-pip -->
    ```
  * Fill the variable-sample file with your details and store it as variables.yml at the same level as main.yml.
    ```shell
    myhostname: xxx.xxx.xxx.xxx
    myusername: xxx
    mypassword: xxx

    nfs_license: xxxxxxxxxxx, xxxxxxxxxxxx 
    cifs_license: xxxxxxxxxxx, xxxxxxxxxxxx 
    flex_license: xxxxxxxxxxx, xxxxxxxxxxxx 
    snapm_license: xxxxxxxxxxx, xxxxxxxxxxxx 
    iscsi_license: xxxxxxxxxxx, xxxxxxxxxxxx 

    node1: xxx
    node2: xxx
    ```

    
