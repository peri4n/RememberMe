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

## TODOs:
* [ ] Create working Docker Image
    * [ ] Choose Base Image
    * [ ] Create Directory
    * [ ] Build App
    * [ ] Run App
* [ ] Mount `build/` dir as a volume?
* [ ] Discuss how to build, run, tag, exec, ... with Docker --> in README
* [ ] Create Service in `docker-compose.yml`
* [ ] Usage of ENV Variables for e.g. Port

