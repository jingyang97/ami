# ami

GitHub repository for AMI

1. set environment variable in your computer, run `packer build` (in my case, I set up project in CircleCi, so it will build automatically when pr merged)
2. trigger build through API is also allowed
3. scp project files, unzip if needed
4. run `mysql.server start`
5. run `scp -r /Users/jingyang/GitHub/webapp.zip awsdev:/home/ubuntu` on local, then `unzip webapp.zip`
6. run `python3 manage.py makemigrations; python3 manage.py migrate; python3 manage.py runserver 0.0.0.0:8000` on the root path of the project
7. open the link, you will see the UI of the web app
