# Registration Service

This is a service to register the reminders, implemented in Spring Boot.

## Running locally
All commands have to be executed in this directory.

Build the app via
```
./gradlew build
```

Run the app (no previous build needed) via
```
./gradlew run
```

See all options for gradle
```
./gradlew tasks
```

## Running in Docker
To be filled

Build and run the container:
```sh
docker build -t foo .
docker -p 8080:8080 foo
```

To debug (also works for layers):
```
docker run -it SHAID /bin/bash
```

## TODOs:
* [ ] Create working Docker Image
    * [x] Choose Base Image
        * Alpine vs Slim vs Default
        * OpenJDK vs AdoptOpenJDK
    * [x] Create Directory
    * [ ] Create seperate User
    * [x] Build App
        * Build Stage to keep the image small, creates JAR
    * [x] Run App
        * Execution Stage, only needs JRE Environment, executes JAR
* [ ] Mount `build/` dir as a volume?
* [x] Discuss how to build, run, tag, exec, ... with Docker --> in README
* [x] Create Service in `docker-compose.yml`
* [?] Usage of ENV Variables for e.g. Port

