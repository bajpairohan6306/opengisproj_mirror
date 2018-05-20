# Disclaimer
This is public mirror to the private project "Opengisproj" created on GitHub under the user @thisisayush forked by @omi10859 with the intention of collaboration and development on the project "Opengisproj". The mirror is created only for referencial purposes and is strictly not meant for redistributing commecially and neither to be procured for personal or commercial use. Aiming to only represent the work done by the collaborators. The development and latest commits for Opengisproj are [here](https://github.com/thisisayush/opengisproj). (Private) 

The work done by the collaborators is to be considered only as v1. This mirror will not be updated further. 
Licensed under GNU General Public License (GPL) v3 or later. Check [COPYING](https://github.com/vipulgupta2048/opengisproj_mirror/blob/master/COPYING) and [LICENSE](https://github.com/vipulgupta2048/opengisproj_mirror/blob/master/LICENSE) for the same. 
For any queries: mailto:vipulgupta2048@gmail.com  

# Yamuna River GIS Project [Private]
GIS Open Source Project  
This project uses Postgresql. Install postgresql server and pgadmin4 for easy management of database during development phase
Edit - First prize awarded in the competition "Making a Web App using GIS and FOSS" 
Thanks for contributing everybody !!

# How to Install

### Create a virtual environemnt to start with.
```
python -m venv VENV_NAME
```

### Clone the repo.
```
git clone https://github.com/YOUR_GITHUB_FORK_URL
```

### Activate the venv
Windows:
```
VENV_NAME/Scripts/activate
```
Linux
```
source VENV_NAME/bin/activate
```
### Install the requirements
Navigate to cloned_repo/
```
pip install -r requirements.txt
```
### Create a .env file
Create a .env file in project_dir/cloned_repo/opengisproj/opengisproj with
following data:
```
DEBUG=true
DATABASE_NAME=your_database_name
DATABASE_USER=your_database_user
DATABASE_PASS=your_database_pass
DATABASE_HOST=your_database_host
DATABASE_PORT=your_database_port
```

### Create the initial database tables
Navigate to cloned_repo/opengisproj/
```
python manage.py migrate
```

### Create the initial superuser
Navigate to clones_repo/opengisproj/
```
python manage.py createsuperuser
```
Fill up the required info

### Start the server
```
python manage.py runserver
```

Check the installation at http://127.0.0.1:8000/
