![plot](TweetAnalyser.png)

Project overview:

  - A web app to analyse streaming data (tweets) by implementing a mesh of microservices using the event-driven architecture. Ensured scalability by implementing CQRS pattern using Kafka and Elasticsearch. 
  - Improved resiliency of microservices by implementing various patterns like externalised configuration, service registration and discovery, API gateway, circuit breaker and rate limiting using Spring Cloud. 
  - Aggregated logs for visualization using the ELK (Elasticsearch, Logstash and Kibana) stack,  implemented authentication and authorization using OAuth 2.0 and OpenID Connect protocols using Keycloak and monitored microservices using Prometheus and Graphana.

# Running the application
- Please enter the correct credentials in twitter4j.properties file in twitter-to-kafka-service 
and enter your github password and url on bootstrap.yml file of config-server
- Then run mvn install -DskipTests command
- Then run docker-compose up command in docker-compose folder
- Check analytics-service, where created an api to be queried for analytics data from query service
