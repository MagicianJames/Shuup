
## Getting Started  
# Install #Python3  
  sudo apt install -y python3-pip  
# Pip package manager for python  
  sudo apt install python3-pip  
# Install Django 
  pip3 install Django  
# Clone:Shuup Template  
  https://github.com/shuup/shuup-project-template 
# Create VirtualEnv to specify dependencies used in the project  
  virtualenv venv

## Start Setting Up Application
# Migreate the Database  
  Install dj-database libraries  
    pip install dj-database-url==0.4.2  
    pip install django-environ  
    pip install easy-thumbnails  
    pip install shuup  

# Copy pasted the template  
* Copy shuup's django template setup to project/settings.py  
    https://github.com/shuup/shuup/blob/master/shuup_workbench/settings/base_settings.py  
* Copy shuup's urls template setup to project/urls.py  
    https://github.com/shuup/shuup/blob/master/shuup_workbench/urls.py  
# Initialize database by running  
  python manage.py migrate

# Initialize installation by running  
  python manage.py shuup_init

## Create superuser with  
  python manage.py createsuperuser

##Start Server by  
  python manage.py runserver 0.0.0.0:8888
