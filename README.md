# machine-learning-project

### Software and account Requirement.

1. [Github Account](https://github.com)
2. [Heroku Account](https://dashboard.heroku.com/login)
3. [VS Code IDE](https://code.visualstudio.com/download)
4. [GIT cli](https://git-scm.com/downloads)
5. [GIT Documentation](https://git-scm.com/docs/gittutorial)


Creating conda environment
```
conda create -p venv python==3.7 -y
```
```
conda activate venv/
```
OR 
```
conda activate venv
```

```
pip install -r requirements.txt
```

To Add files to git
```
git add .
```

OR
```
git add <file_name>
```

> Note: To ignore file or folder from git we can write name of file/folder in .gitignore file

To check the git status 
```
git status
```
To check all version maintained by git
```
git log
```

To create version/commit all changes by git
```
git commit -m "message"
```

To send version/changes to github
```
git push origin main
```

To check remote url 
```
git remote -v
```

To setup CI/CD pipeline in heroku we need 3 information
1. HEROKU_EMAIL = amr.alkamel.m3@gmail.com
2. HEROKU_API_KEY = <>
3. HEROKU_APP_NAME = ml-regression-model

BUILD DOCKER IMAGE
```
docker build -t <image_name>:<any tagname> .
```
> Note: Image name for docker must be lowercase


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

Tos stop docker conatiner
```
docker stop <container_id>
```



```
python setup.py install
```

[teacher github repo](https://github.com/avnyadav/machine_learning_project)


Pickle
```
import pickle
```
>it is used to save any kind of class objects. 
>Saving object to a file is called seriliazation (pickle.dump())
>Loading any object from a file is called deseriliazation


Hash Data Integrity

> It is used to check data versioning, to check if data has been changed or not. 
>You basically generate a hash value for your data, then after sometime you well check if this value has been changed, if so the data is also changed.


Artifact

> It is defined for all components separately and it expresses the output.
> It is the output of each component and it is named based on the components names.

Config
> It is created separately for each component and it expresses the input.
> The artifact of the previous component is considered as the config of the next component. 