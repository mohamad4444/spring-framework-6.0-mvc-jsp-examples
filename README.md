# Spring MVC JSP Examples

A collection of traditional Spring MVC learning examples with JSP views and XML
configuration, kept as a reference for how a manually configured Spring web
application is structured. This project does not use Spring Boot.

## Examples and structure

- Annotated MVC controllers and model attributes in `src/main/java/com/telusko/controllers/`.
- Form binding, validation, grocery items, and file upload examples.
- JSP views with Spring form tags and JSTL in `src/main/webapp/`.
- Explicit `DispatcherServlet` and application context setup in `src/main/webapp/WEB-INF/web.xml`.
- Component scanning and message source configuration in `src/main/webapp/WEB-INF/spring-config.xml`.

## Version and build snapshot

The traditional structure does not indicate the Spring version: the current
`pom.xml` declares Spring Framework **6.0.9**, Spring Security **6.1.0**, and Java
source/target **19**. The original version notes also discuss Spring 4 and 5.

This is a learning snapshot with mixed configuration: the POM includes both
`javax.servlet` and `jakarta.servlet` APIs, controllers still import
`javax.servlet`, and `web.xml` declares Servlet 4.0. Maven packaging is currently
the default JAR despite the web application layout. Runtime compatibility and
deployment setup need review before treating it as a runnable template.

The Maven artifact and local Eclipse project/context name are
`spring-mvc-jsp-examples`. Dependencies and application behavior have not been
modernized as part of the rename.

The [original version notes](docs/legacy-version-notes.md) are preserved as
historical material rather than current setup instructions.

Previously stored locally as `AC-YT-myapp2_git`.
