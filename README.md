# personal-home-stuff

Miscellaneous automation for daily living.

Currently this includes some automation to load some favorite tunes on a USB drive for easy access in the car.

## Project Setup

Assumes Ansible is installed, on a Linux or OSX workstation.

If ansible is not installed, try this:
(Ubuntu 14.04)

``` bash
sudo apt-add-repository ppa:ansible/ansible
sudo apt-get update
sudo apt-get install ansible
```

(Ubuntu 16+)

``` bash
sudo apt install -y python-pip git
sudo pip install ansible
```

(OSX)

``` bash
brew install ansible
```

## Running the Code

* Install git (if you haven't already) `sudo apt-get install git` or `brew install git`
* Clone this repo: `git clone https://github.com/huxoll/personal-home-stuff.git`
* (Or, clone the repo via SSSH: `git clone git@github.com:huxoll/personal-home-stuff.git` with appropriate SSH key)
* Change to the directory: `cd personal-home-stuff`
* Copy the example inventory file and customize variables: `cp inventory.sample inventory && vi inventory`
* Copy the example extra variables file and customize variables if you wish: `cp extra_vars.yml.sample extra_vars.yml &&
 vi extra_vars.yml`
* Run `ansible-playbook -i inventory --extra-vars "@extra_vars.yml" carstick.yaml`.
