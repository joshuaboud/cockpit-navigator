# Cockpit Navigator
A Featureful File System Browser for Cockpit - remotely browse, manage, edit, upload, and download files on your server through your web browser.  

## Features
With no command line use needed, you can:
* Navigate the entire filesystem,
* Create, delete, and rename files,
* Edit file contents,
* Edit file ownership and permissions,
* Create symbolic links to files and directories,
* Reorganize files through cut, copy, and paste,
* **Upload files by dragging and dropping**,
* **Download files and directories**.

| Browsing Filesystem |
|---------------------|
| ![User Interface](doc/ui_root.png) |

| Editing Content | Editing Properties | 
|-----------------|--------------------|
| ![Edit Contents](doc/ui_editor.png) | ![Edit Preferences](doc/ui_prefs.png) |

# Installation
## From Github Release
### Ubuntu
1. `$ wget https://github.com/45Drives/cockpit-navigator/releases/download/v0.5.3/cockpit-navigator_0.5.3-1focal_all.deb`
1. `# apt install ./cockpit-navigator_0.5.3-1focal_all.deb`
### EL7
1. `# yum install https://github.com/45Drives/cockpit-navigator/releases/download/v0.5.3/cockpit-navigator-0.5.3-1.el7.noarch.rpm`
### EL8
1. `# dnf install https://github.com/45Drives/cockpit-navigator/releases/download/v0.5.3/cockpit-navigator-0.5.3-1.el8.noarch.rpm`
## From Source
1. Ensure dependencies are installed: `cockpit`, `python3`, `rsync`, `zip`.
1. `$ git clone https://github.com/45Drives/cockpit-navigator.git`
1. `$ cd cockpit-navigator`
1. `$ git checkout <version>` (v0.5.2 is latest)
1. `# make install`
## From 45Drives Repositories
### Ubuntu
1. Import GPG Key
```sh
wget -qO - http://repo.45drives.com/key.asc | sudo apt-key add -
```
2. Add 45drives.list
```sh
cd /etc/apt/sources.list.d
sudo wget http://repo.45drives.com/debian/45drives.list
sudo apt update
```
3. Install Package
```sh
sudo apt install cockpit-navigator
```
### EL7/EL8
1. Add Repository
```sh
cd /etc/yum.repos.d
sudo wget http://repo.45drives.com/rhel/45drives.repo
sudo yum clean all
```
2. Install Package
```sh
sudo yum install cockpit-navigator
```
