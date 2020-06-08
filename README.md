# ami
GitHub repository for AMI

1. set environment variable in your computer, run `packer build` (in my case, I set up project in CircleCi, so it will build automatically when pr merged)
2. scp project files, unzip if needed
3. run `mysql.server start`
4. run `python3 manage.py makemigrations; python3 manage.py migrate; python3 manage.py runserver 0.0.0.0:8000`
5. open the link, you will see the UI of the web app
