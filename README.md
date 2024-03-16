# VS_code_prax

This is our project root folder. ReadMe.md  file is typically the first file to create and should contain a brief description of the project and high-level overview. 

# secret key should be changed and kept secret, not published to github 
docker run -d -p 8080:8088 -e "SUPERSET_SECRET_KEY=asdfghjkl" --name superset apache/superset

docker exec -it superset superset fab create-admin \
              --username admin \
              --firstname Superset \
              --lastname Admin \
              --email admin@superset.com \
              --password admin


docker exec -it superset superset db upgrade

docker exec -it superset superset init


not running examples for now..
docker exec -it superset superset load_examples

Edit Dockerfile to include the important content then run:
docker build -t my/superset:duckdb


docker run -d -p 8080:8088 -v $PWD:/data:rw -e "SUPERSET_SECRET_KEY=asdfghjkl" --name superset my/superset:duckdb

Now we're learning about git and how git tracks file in our project folder.

testib giti