docker : 
docker pull mongodb/mongodb-community-server:latest
docker run --name mongodb -p 27017:27017 -d mongodb/mongodb-community-server:latest

neo4j: 
docker pull neo4j
docker run --name myneo4j -p 7687:7687 -p 7474:7474 -d -e NEO4J_AUTH=neo4j/password neo4j:latest
