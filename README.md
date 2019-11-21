# Fun with Airflow
This repo has been set up to allow you to quickly get Airflow up and running on your computer using docker.
Then you can add your own dags and run and test some basic workflows.

# Run on your own machine:
Clone this and run the following command, you'll need `docker` and `docker-compose`
Follow [docker compose](https://docs.docker.com/compose/install/) and [docker ce (community edition)](https://docs.docker.com/install/#supported-platforms) install instructions to get these.

Then run `sh build_all_dockers.sh` to build all the relevant docker files.

+ WebserverDockerfile - is airflow webserver
+ SchedulerDockerFile - is airflow scheduler
+ PostgresDockerFile - is postgres database used for scheduler and webserver data storage

then do `docker-compose -f docker-compose-LocalExecutor.yml up`

