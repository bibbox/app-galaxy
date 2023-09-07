# Galaxy BIBBOX application

Bibbox compatible version of [Galaxy docker](https://github.com/anvilproject/galaxy).

## Hints
* approx. time with medium fast internet connection: **15 minutes**

## Install within BIBBOX

Within BIBBOX you can use the [BIBBOX](https://bibbox.readthedocs.io/en/latest/ "BIBBOX") to install a lot of software tools. After the installation is finished you can start your application in the dashboard.

### Install Environment Variables

 * ADMIN_USERS = admin username\
You can set the admin username. After the installation is completed you should immediately register a new user with your chosen admin username. This user will automatcally be the admin user. NOTE: Anyone can register an adminuser if they know the admin username right after the installation. 

## Docker Images Used
 * galaxy/galaxy-anvil

## Standalone Installation

To install the app locally execute the commands:
* Clone the git repository: 
  * `git clone https://github.com/bibbox/app-galaxy.git`
* Change the current directory to app-molgenis: 
  * `cd app-galaxy/` 
* Create the docker network `bibbox-default-network`: 
  * `docker network create bibbox-default-network`
* Run **docker-compose up** in the root folder of the project: 
  * `docker-compose up -d`
* **Alternatively** on a *Linux* system run the bash script `intsall.sh` after cloning and change the working directory to the git repository directory.
 


## Mounted Volumes
 * ./data/database

## TODOS
 * Enable FTP/SFTP connection
