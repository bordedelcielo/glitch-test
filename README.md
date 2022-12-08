# Deploy Flask Application to Glitch #

glitch.com
import public repo

- Create a gunicorn.conf.py file

        workers = 5
        bind = "0.0.0.0:8080"
- Create a script file, start.sh. If you have ever deployed to Heroku, this essentially replaces the Procfile.

        gunicorn "app:create_app()"
- Open glitch's Terminal and enter the below command:

        pip3 install -r requirements.txt
- Click into glitch's .env file and load it with the applications environment variables.

Fantastic! Project deployed.