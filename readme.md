## Docker

Based on the following conditions, set up a Dockerfile for the Java application downloaded from 

* It should use Java 1.8
* The command to launch the application is: `java -jar gs-spring-boot-0.1.0.jar`
* The default port should be 80 (use the `SERVER_PORT` environment variable)
* Expose the default port
* There should be an environment variable for `NAME` with default `unknown`

Optional: Set up a Docker Compose file that spins up the Java application, with a containerized nginx proxy in front of it.
# containerized-java-application
