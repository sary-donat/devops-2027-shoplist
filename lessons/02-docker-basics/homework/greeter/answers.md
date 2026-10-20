docker build -t greeter:v1
docker run -d --name greeter -p 9000:8080 greete:v1
docker rm -f greeter  ->  docker run -d --name greeter -p:8080 -e GREETING=Shalom  greete:v1
Shalom Rivka
from COPY . 
