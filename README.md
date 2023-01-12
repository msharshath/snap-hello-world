## How to build, install and run the hello-world snap on Ubuntu:

### Install snapcraft
```
sudo snap install snapcraft --classic
```
### Install lxd
```
sudo snap install lxd
```
### Install git 
```
sudo apt update
sudo apt install -y git
```
### Clone repo
```
cd ~/
git clone https://github.com/ernestl/snap-hello-world.git
```
### Build hello-world snap in lxd container
```
cd ~/snap-hello-world
snapcraft --use-lxd --debug
```
### Install snap (note: this is a development mode snap)
```
sudo snap install hello-world_0.1_amd64.snap --devmode --dangerous 
```
### Run the application
```
hello-world
```
