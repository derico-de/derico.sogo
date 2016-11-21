# derico.sogo


An Ansible Playbook to build, install and configure SOGo 32bit on Debian
jessie.

## Usage


      roles:
        - role: derico.sogo
          sogo_pg_user: sogo
	  tags:
	    sogo

### Define SOGo PostgreSQL DB password in a vault encrypted file

The default PostgreSQL password is 'xxx', but it's highly recommended to define a new one in a ansible-vault encrypted file. The variable name is sogo_pg_pw.

