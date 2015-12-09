How to install
--------------

    ansible-galaxy install -r requirements.yml

with the content of requirements.yml
    
    
    # requirements.yml
    
    - src: https://github.com/vantt/ansible_memcached.git
      version: master
      name: memcached_role

How to use
----------

    # playbook.yml
    
    - hosts:  all 
      sudo: yes
      gather_facts: true
      roles:
        - { role: memcached_role }
