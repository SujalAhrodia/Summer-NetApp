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
  * Install pip for python2 
    ```shell
    $ sudo apt install python-pip
    ```
  * Fill the variable-sample file with your details and store it as variables.yml at the same level as main.yml.
    ```shell
    hostname: XXXX
    username: XXXX
    password: XXXX
    vserver: XXXX
    node1: XXXX
    node2: XXXX
    vol: XXXX
    vol2: XXXX

    nfs_license: XXXXXXX
    cifs_license: XXXXXX
    flex_license: XXXXXX
    snapm_license: XXXXXX
    ```

    
