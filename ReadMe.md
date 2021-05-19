# Run Elasticsearch with Kibana from Docker

- Download the docker compose file.
- Make the changes based on your local directory where you want to persist your data.
- Make changes to specific versions of elasticsearch or Kibana based on your need.
- Go to the folder you have docker compose file in command prompt and run below command.
`docker-compose up -d`
- Now you can close the command prompt since we are running it in non-interactive mode.
- Use following curl command to verify if the elasticsearch node is up and running.
`curl http://127.0.0.1:9200/_cat/health`
You will get a similar response as following: `1621357151 16:59:11 docker-cluster green 1 1 7 7 0 0 0 0 - 100.0%`
This gives information on cluster name "docker-cluster" and status "green".
- You can also access you Kibana using `http://localhost:5601/`
