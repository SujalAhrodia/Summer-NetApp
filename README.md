<img src="http://www.freelogovectors.net/wp-content/uploads/2018/04/netapp-logo.png" width="300"> 

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
    netapp_hostname: XXXX
    netapp_username: XXXX
    netapp_password: XXXX
    netapp_vserver: XXXX
    netapp_node1: XXXX
    netapp_node2: XXXX
    netapp_vol1: XXXX
    netapp_vol2: XXXX

    nfs_code: XXXXXXX
    cifs_code: XXXXXX
    flex_code: XXXXXX
    snapm_code: XXXXXX
    ```

    
