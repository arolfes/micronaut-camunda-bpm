# example-standalone-cockpit

This example demonstrate how to use micronaut-camunda-bpm to run camunda cockpit as standalone app with disabled job executors

## Start the application

### start microservice with process and enabled process engine

as first step we need to start another micronaut app which implements the process and process engine

```bash
cd ../example-external-task-process
docker-compose up

../gradlew :example-external-task-process:run
```

### start standalone camunda cockpit

```bash
../gradlew run
```