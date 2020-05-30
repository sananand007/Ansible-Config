## Repository of Ansible Playbooks


### Process

#### Connect and ping the DO instances

- connect through SSH and verify all the ansible hosts that will be used as slaves
    ```
    ssh -i <private_key> root@ip
    ```
- use the correct ansible inventory file and ping verify all the droplets
- Remember to chagne the user to something other than root user as that is not very secure
- Ping verification can be done as below for the root user
    ```
    ansible all -m ping -u root

    ```

- start_terminate_ec2
-   This will start Create a new EC2 instance, launch instance, Add instance to a hostgroup, wait for SSH to come up, configure, Terminate the instance

