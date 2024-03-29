# account
This application was generated using JHipster 4.13.0, you can find documentation and help at [http://www.jhipster.tech/documentation-archive/v4.13.0](http://www.jhipster.tech/documentation-archive/v4.13.0).

This is a "microservice" application intended to be part of a microservice architecture, please refer to the [Doing microservices with JHipster][] page of the documentation for more information.

This application is configured for Service Discovery and Configuration with . On launch, it will refuse to start if it is not able to connect to .

## Development

To start your application in the dev profile, simply run:

    ./mvnw


For further instructions on how to develop with JHipster, have a look at [Using JHipster in development][].



## Building for production

To optimize the account application for production, run:

    ./mvnw -Pprod clean package

To ensure everything worked, run:

    java -jar target/*.war


Refer to [Using JHipster in production][] for more details.

## Testing

To launch your application's tests, run:

    ./mvnw clean test
### Other tests

Performance tests are run by [Gatling][] and written in Scala. They're located in [src/test/gatling](src/test/gatling) and can be run with:

    ./mvnw gatling:execute

For more information, refer to the [Running tests page][].

## Using Docker to simplify development (optional)

You can use Docker to improve your JHipster development experience. A number of docker-compose configuration are available in the [src/main/docker](src/main/docker) folder to launch required third party services.

You can also fully dockerize your application and all the services that it depends on.
To achieve this, first build a docker image of your app by running:

    ./mvnw verify -Pprod dockerfile:build

Then run:

    docker-compose -f src/main/docker/app.yml up -d

For more information refer to [Using Docker and Docker-Compose][], this page also contains information on the docker-compose sub-generator (`jhipster docker-compose`), which is able to generate docker configurations for one or several JHipster applications.

## Continuous Integration (optional)

To configure CI for your project, run the ci-cd sub-generator (`jhipster ci-cd`), this will let you generate configuration files for a number of Continuous Integration systems. Consult the [Setting up Continuous Integration][] page for more information.

[JHipster Homepage and latest documentation]: http://www.jhipster.tech
[JHipster 4.13.0 archive]: http://www.jhipster.tech/documentation-archive/v4.13.0
[Doing microservices with JHipster]: http://www.jhipster.tech/documentation-archive/v4.13.0/microservices-architecture/
[Using JHipster in development]: http://www.jhipster.tech/documentation-archive/v4.13.0/development/
[Using Docker and Docker-Compose]: http://www.jhipster.tech/documentation-archive/v4.13.0/docker-compose
[Using JHipster in production]: http://www.jhipster.tech/documentation-archive/v4.13.0/production/
[Running tests page]: http://www.jhipster.tech/documentation-archive/v4.13.0/running-tests/
[Setting up Continuous Integration]: http://www.jhipster.tech/documentation-archive/v4.13.0/setting-up-ci/

[Gatling]: http://gatling.io/
