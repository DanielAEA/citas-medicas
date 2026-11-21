# citas-medicas

Proyecto del taller de pruebas de software en Spring Boot (Java 25, Spring Boot 4.0.0, Maven).

## Ejecutar la aplicación

    mvn spring-boot:run

Abrir http://localhost:8080/citas.html

## Pruebas

    mvn -Dtest=AgendaServiceTest test
    mvn -Dtest=CitaControllerTest test
    mvn -Dtest=CitaRepositoryTest test
    mvn -Dtest=ReservaIntegracionTest test
    mvn clean test
    mvn verify

El reporte de cobertura queda en target/site/jacoco/index.html. Las pruebas de interfaz (ReservaUITest, etiquetadas ui) se ejecutan de forma individual y requieren Google Chrome.
