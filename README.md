
#heroku

-Creating an app on Heroku
heroku apps:create node-api-docker-heroku 

-Change to container because is necessary to work with Docker
heroku stack -a <nome-app>
heroku stack:set container -a <nome-app>

-Push to Heroku
git push heroku main
git push heroku <branch>:main

-Verify logs
heroku logs -t --app APP_NAME

-Set enviroment variables
heroku config:set <VARIABLE>=<value> --app NOME_DO_APP
