# Boston House Pricing Prediction

### Software And Tools Requirements

1. [Github Account](https://github.com)
2. [HerokuAccount](https://heroku.com)
3. [VSCodeIDE](https://code.visualstudio.com/)
4. [GitCLI](https://git-scm.com/book/en/v2/Getting-Started-The-Command-Line)

Create a new environment

```
conda create -p venv python==3.7 -y
```
activate the environment using the following command
```
conda activate venv
```

Create a requirements.txt file
```
touch requirements.txt
```
add necessary modules into requirements.txt file
install it by using the following command
```
pip install -r requirements.txt
```

configure GitHub in terminal
```
git config --global user.name "github_user_name"
git config --global user.email "github_created_mail"
```

created  model and scaling pickle files from ipynb notebook
with that model predcting the data

created a html page in template folder

add the Dockerfile 
```
FROM python:3.7
COPY . /app
WORKDIR /app
RUN pip install -r requirements.txt
EXPOSE $PORT
CMD gunicorn --workers=4 --bind 0.0.0.0:$PORT app:app
```

create main.yaml file inside .github/workflows folder

