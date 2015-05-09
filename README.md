# How to run this code?
You'd need to install these on your workstation:
* [Vagrant](https://www.vagrantup.com/downloads.html)
* [Ansible](http://docs.ansible.com/intro_installation.html)
* [git](http://git-scm.com/)

If you're using a Mac, you can use [Homebrew](http://brew.sh/):

```bash
# Installing Homebrew
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

```bash
# Install vagrant with Virutalbox provider
brew install brew install caskroom/cask/brew-cask
brew cask install virtualbox
brew cask install vagrant
```

```bash
# Install Ansible
brew install ansible
```

```bash
# Install git
brew install git
```

Once all is installed, just clone this repo and start the vagrant box:

```bash
git clone https://github.com/navidpaya/challenge.git
cd challenge
vagrant up
```

Port 8000 of the nginx server on the vagrant box is mapped to port 8000 on your workstation, so once done with the run, just open your browser and go to:

http://localhpst:8000/
