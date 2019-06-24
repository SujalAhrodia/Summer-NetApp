# Summer-NetApp

1. Setting up the environment
  * Cluster with an HA pair running ONTAP 9.5
  * Jumphost, Ubuntu-18.04.1-desktop-amd64
2. On the jumphost:
  * Clone the repo
    ```shell
    $ git clone https://github.com/SujalAhrodia/Summer-NetApp.git
    ```  
  * Install the latest version of ansible(atleast 2.6)
    ```shell
    $ sudo apt update 
    $ sudo apt-add-repository ppa:ansible/ansible
    $ sudo apt install ansible
    ```
  * Install pip for python2 and python3
    ```shell
    $ sudo apt install python-pip
    $ sudo apt install python3-pip
    ```


    
