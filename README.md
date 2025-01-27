1. **Stage 0: Init manager host**

- SSH as root
- Install needed packages to start the setup
    ```bash
    apt get install ansible git
    ```
- Clone the public repository 
    ```bash
    cd /root
    git clone https://github.com/kdev-labs/sysadm-init.git
    git clone git@github.com:kdev-labs/sysadm-init.git
    ```
- Run the init.yaml playbook create local users kregez/sysadm for further setup
    ```bash
    ansible-playbook sysadm-init/init.yaml --connection=local
    ```

- Continue setup in https://github.com/kdev-labs/sysadm