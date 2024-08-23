# ansible

* ansible configurations

* create one user call `devops`
* give the permisson user `devops`, `sudo visudo`
* configuration on `vi /etc/ssh/ssh_config` and `vi /etc/ssh/sshd_config.d/60`
* after excute this command `sudo systemctl restart ssh.service`
* create key in master node `ssh-keygen`
* copy the key form `ssh-copy-id `

* create *hosts* file on matenode `vi hosts`


```
    ansible -i hosts -m ping all
    ansible-playbook -i apply -f hosts <demo.yaml>
```

