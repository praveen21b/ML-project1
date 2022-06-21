# ML-project1

## Requirements
1.  Github account
2.  Heroku accountconda activate
3.  VS code IDE
4.  GIT cli

## Steps

Creating conda virtual environment
```
conda create -p ml1 python==3.8 -y
```

```
conda activate ml1 or conda activate ml1/
```

```
pip install -r requirements.txt
```

Adding files to the git hub
```
git add <file_name>
```
OR
```
git add .
```

Note: to ignore files/ folders saving to the git by adding names in .gitignorefile

to check git status
```
git status
```

to check versions maintined by git
```
git log
```

to create versions/ commit all  the changes by git
```
git commit -m "message to display"
```

to send version/changes to the github
```
git push origin main
```

to remote url
```
git remote -v
```

## Setup CI/CD pipeline
We need 3 information to setup CI/CD in heroku
1.  Heroku email = praveen.h119@gmail.com
2.  Heroku API_key = 1465a4fb-a6e3-4dd0-8b08-c5aac77209f6
3.  Heroku app name = ml1-hello-world

BUILD DOCKER IMAGE
```
docker build -t <image_name>:<tagname>
```
Note: Image name for docker must be lowercase

To list docker image
```
docker images
```

Run docker image
```
docker run -p 5000:5000 -e PORT=5000 f8c749e73678
```

To check running container in docker
```
docker ps
```

To stop docker conatiner
```
docker stop <container_id>
```
python setup.py install