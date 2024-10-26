# Curso de Grado - Taller de Desarrollo y Producción de Software

1. **Conceptos sobre Arquitectura de Software**: Definición (o mejor dicho definiciones). Visualización de la arquitectura de software de un sistema, principalmente con el [modelo C4](https://c4model.com/) de Simon Brown. Arquitecturas monolíticas vs distribuídas. Arquitecturas monolíticas modulares y microservicios. Atributos de calidad: mantenibilidad, escalabilidad y disponibilidad. Contenidos obtenidos de mi libro [Coding An Architecture Style](https://leanpub.com/codinganarchitecturestyle), que por supuesto **es gratis para mis alumnos** y cualquiera que quiera leerlo.
2. **Arquitectura Web**: El protocolo HTTP, Servicios HTTP y Servicios REST. Aplicaciones Web Single Page.
3. **Integración Continua y Calidad**: Desarrollando en equipo necesitamos configurar un robot que verifique la calidad del código producido por cada integrante. Por eso utilizaremos:

- [Checkstyle](https://maven.apache.org/plugins/maven-checkstyle-plugin/examples/custom-checker-config.html). Utilizamos la guía de estilos de [Google](https://google.github.io/styleguide/javaguide.html).
- [PMD](https://maven.apache.org/plugins/maven-pmd-plugin/). Utilizamos las siguientes reglas [PMD Rules](https://pmd.github.io/latest/pmd_rules_java.html), excepto las relacionadas con la documentation (javadoc).
- [Spotbugs](https://spotbugs.github.io/spotbugs-maven-plugin/). Éstas son las reglas que spotbugs verifica: [Spotbugs Rules](https://spotbugs.readthedocs.io/en/stable/bugDescriptions.html).
- [Jacoco](https://www.eclemma.org/jacoco/trunk/doc/maven.html) para generar reportes de covertura de código. Luego, enviamos los reportes mediante una acción de Github a [Codecov](https://about.codecov.io/), para mostrar el badge con el porcentaje de covertura.
- [Code Climate](https://codeclimate.com/), otro analizador de código estático que ranquea nuestros fuentes segun métricas específicas.

4. **NoSQL** y **NewSQL**: ¿Qué motivó su aparición?. Consistencia. Teorema de CAP y Conceptos Básicos de Arquitecturas Distribuídas. Escalar en Bases de Datos Relacionales y en Base de Datos NoSQL. Arquitecturas Master-Slave. Sharding. Familias de BDs NoSQL: Conceptos sobre almacenamiento de tipo Clave-Valor (Redis), Documento (MongoDB), Familia de Columnas (Cassandra) y Grafos (Neo4J / Gremlin). Usos adecuados de cada uno. Comparación con usos adecuados de bases de datos relacionales.

## ¿Queres correr este proyecto?

1. clonalo y luego:
2. npm install
3. npm start

Los contenidos de este curso estan desarrollados utilizando el hermoso framework [Reveal.JS](https://revealjs.com/).
s