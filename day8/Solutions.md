DAY 8 ANSIBLE

Assignment 1

1. Create 5 users with password, and these five users should have same permissions for a directory named ninja.(Directory can be created with the 5 users permmission.)

2. Create ssh key for each user so that all those 5 users will be able to login through ssh.

Solution :-

Created 5 users

- Created a playbook named Usermanagement.yml

- For permission we can use ACL module in ansible

 - name: Grant user Joe read access to a file
 ```
    acl:
                 path: /home/vagrant/common_dir
                 entity: common_dir
                 etype: directory
                 permissions: r+w
                 state: present
```
Usermanagement Playbook


Usermanagement run





3. Creat Logical Volume in any node machine.

4. need to installl lvm2 first using ansible.

5. Create ext4 type File System on the newly created logical volume.

6. Mount newly created file system.

LVM YML


LVM RUN


STEPS:-
1.

2.

3.

4.

5.

6.

7.

8.

9.

10.