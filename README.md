# personal-home-stuff
Miscellaneous automation for daily living.

# Project Setup
All required packages that ansible needs, as well as ansible can be installed via scripts
in this repo. The dependencies are in a python_requirements.txt file located at:

```
extensions/setup/python_requirements.txt
```

# Running the Code
Code in this repo is functional and tested. To run it, you need to install ansible and all the dependencies. You can do this simply by executing:

```
./extensions/setup/setup.sh
```

* If you already have ansible, and you do not want to go through the installation simply create a vpass text file in the root directory and add the secret code (123456)
* To install roles execute the role_update.sh which will download all the roles
```
./extensions/setup/role_update.sh
```
* Go to the plays directory and then execute and do not forget to change the host address in the development.ini
```
ansible-playbook -i ../development.ini carstick.yml
```

