### 2 ways to build this:

## Run on your own machine:
Clone this and run the following command, you'll need `docker` and `docker-compose`
Follow [docker compose](https://docs.docker.com/compose/install/) and [docker ce (community edition)](https://docs.docker.com/install/#supported-platforms) install instructions to get these.

Then run `sh build_all_dockers.sh` to build all the relevant docker files.

+ WebserverDockerfile - is airflow webserver
+ SchedulerDockerFile - is airflow scheduler
+ PostgresDockerFile - is postgres database used for data (not airflow) webserver

then do `docker-compose -f docker-compose-LocalExecutor.yml up`

