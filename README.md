# Setup
To run the client and API, follow these steps:

1. Untar the Odyssey statistics tarball into the `./data` folder
2. Run the system using docker-compose, i.e. `docker-compose up -d`

# Updating the federation
- Before running the API, you should update the `docker-compose.yml` file to reflect the available sources and their corresponding endpoint
- By convention, the endpoints of sources specified in the `SOURCES` environment variable are upper-cased, e.g. the endpoint of DBpedia is specified with the environment variable `ENDPOINT_DBPEDIA`

# Important directories
- The API source is located at `./api/pipe`
- The client source is located at `./client/src`

# Todos
- Include engine dependency compilation as part of the API Dockerfile
- Add a lock to ensure only one query is executed at once
