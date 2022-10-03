# Roadmaps to web development

## HTTP and networks 

* Internet (creation, concept, operation)
   * Protocol (concept, types, RFC)
   * ISO-OSI levels
   * TCP (concept, utility, well-known ports, structure of TCP segments, sockets)
   * IP (concept, utility, IP addresses, routing, structure of IP datagrams)
   * Client-server applications vs P2P
   * HTTP protocol
     * concept, utility, characteristics, requests and responses
     * HTTP is a stateless protocol
     * structure of an HTTP request and response packet
     * HTTP methods and their utility
     * HTTP response codes
     * URL (concept, structure, parameters)  
   * The process of loading a web page
   * What are MIME types and what are they for?
   * Web sessions
     * Cookies
       * What is a cookie and what is it for? 
       * How can we establish a session using cookies? 
       * where does the cookie travel within the HTTP packet?
     * Tokens: JWT (JSON Web Tokens)
     * Oauth


## Web Projects

   * Requirements, specifications of an application
   * Software development methodologies:
     * Cascade model
     * Spiral model
     * Models based on prototypes
     * Agile methodologies:
       * Kanban methods
       * Extreme Programming
       * Scrum (concept, kanban method, sprints, burnout diagram, tools)
   * Continuous integration (concept, servers)
     * Unit testing concept (concept, tools, mock)
     * Integration testing concept (concept, tools)
     * TDD: Test Driven Development
   * Program documentation (concept, types, tools)
   * Deployment in production and in test. Automated deployment. Cloud deployment.
   * Containers.
     * Docker
     * Docker compose
     * Orchestration
   * Version managers (concept, tools and features)
   * Code repository (types, tools)
   * Software quality assessment (concept, available tools)

## Infrastructure

   * IDES:
     * Java: NetBeans, Eclipse, IntelliJ, VSC
     * Javascript: Visual Studio Code, Sublime, Atom, webstorm
   * Browsers:
     * Chrome, Firefox, Edge, Safari, Opera...
     * Support:
       * https://caniuse.com/
       * https://kangax.github.io/compat-table/es6/
      
## Web Application Design

   * Server API. Endpoints.
   * Entity relationship diagram.
   * Normalization: First, second and third normal forms.
   * Integrity constraints.
   * DB vs. DBMS - DBRMS.
   * DML - DDL: SQL.
   * noSQL (concept and tools).
   * UML: Process diagram.
   * Client mockups, wireframers, prototyping.
   * Navigation diagram of a website.

## Web Application Development
  * Markup languages: HTML, CSS, XML, JSON
  * CSS:
    * CSS frameworks: Bootstrap, Materialize, Foundation, Bulma, Tailwind, Semantic UI, Ulkit
    * CSS Precompilers: Sass and Less
    * BEM
  * Regular expressions.
    * Concept
    * Cheet sheets
    * Links to learn regular expressions
    * Links to online tools to build and validate regular expressions
  * JSON:
    * Concept
    * Cheet sheets
    * Online parser
    * Java JSON converter libraries: Google Gson, Jackson, Moshi...     
  * CDN
  * AJAX
  * Static pages vs dynamic pages
  * Websocket technology
  * Development patterns: MVC, singleton, factory
  * Callback concept
  * CORS
  * Ecmascript: version history
  * Polyfills
  * Asynchronous processing, Callbacks, callback hell, promises and reactive programming
  * Reactive functional programming: RxJS
  * Microservices
  * Differences between CMS, ERP and CRM
  * Important CMS:
    * PHP: Wordpress, Joomla, Drupal, Magento, Prestashop
    * Java: Liferay, OpenCMS, Alfresco, Magnolia, Bynder
  * Major ERPs: SAP, Microsoft Dynamics, JDEdwards, Sage
  * CRM: Salesforce, Zoho, Agile CRM, Close


## Programación y organización del código

  * Concepto de código spaguetti. Explicar porqué se necesita una estructuración en el código.
  * Concepto de abstracción en programación
  * Paradigmas de la programación:
    * ¿En qué consiste paradigma declarativo frente al paradigma imperativo?
    * ¿Qué es la programación funcional y en qué se diferencia respecto de la programación imperativa?
  * Técnicas de programación imperativa
    * Programación estructurada
    * Programación modular: 
      * Acoplamiento y cohesión entre módulos
    * Programación orientada a objetos. Conceptos a desarrollar:
      * Principios SOLID
      * Interfaces, 
      * Clases:
        * Clases abstractas
        * Propiedades y Métodos: Visibilidad de los métodos y de las propiedades, 
        * Implementación de interfaces
      * Concepto de encapsulación 
      * Objetos.
      * Herencia: Concepto de Sobreescribir un método.
      * Concepto de Polimorfismo:
        * polimorfismo basado en implementación de interfaces 
        * polimorfismo basado en la herencia.
    * Particularidades de la orientación a objetos en Javascript
    * Explica en qué consisten las Interfaces fluidas.
    * Qué es la Inyección de dependencias o inversión del control y qué ventajas aporta su uso en la programación web.
    * Qué es la programación orientada a aspectos y qué ventajas aporta su uso en la programación web.
    * ¿Para qué sirven las excepciones y su tratamiento en un programa?
    * Patrones de programación
      * MVC
      * Singleton
      * Factory
      * otros patrones
    * Programación dirigida por eventos y Programación asíncrona
      * Concepto de promesa
      * Concepto de callback
      * Métodos en programación en entorno cliente para manejar la asincronía:
        * Callbacks: infierno callback
        * Promesas
        * Métodos async/await
        * Programación funcional reactiva y RxJs
    * Genericidad del código: Explica la siguiente regla: 
      * Cuanto más genéricos son los programas, más reusable es el código pero también es más complejo y difícil de mantener.



## Lenguajes de programación
  * Lenguajes de programación:
    * lenguajes compilados vs interpretados diferencias y lista de lenguajes)
    * Diferencias entre un Compilador, un interprete y un transpilador
  * Lenguajes débilmente tipados vs lenguajes fuertemente tipados: diferencias, ventajas y desventajas.
  * ¿Qué diferencia existe entre un tipado estático y uno dinámico?
  * ¿Qué es el timetomarket de un lenguaje?
  * ¿En qué consiste el type typing?
  * ¿Qué es la sobrecarga de operadores?
  * ¿Qué es la interpolación de cadenas?
    * Ejemplos de interpolación en Java y Javascript




## Entorno cliente
  * Navegadores: Mosaic, Netscape, Chrome, firefox, Opera, Safari, Internet Explorer, Edge, Vivaldi, Brave
    * el inspector de chrome y firefox
    * manejo de la caché en navegadores
    * el local storage
  * Librerías: jQuery, Prototype, Dojo, Yui
  * Librerias de programación funcional: underscore, lodash, rambda
  * Frameworks de entorno cliente: Backbone, Knockout, Ember, AngularJS, Angular, React, VueJS
  * Diferencias entre una librería y un framework
    * https://stackoverflow.com/questions/148747/what-is-the-difference-between-a-framework-and-a-library#answer-15600924
  * Sistemas de gestión de dependencias: bower, npm, yarn
  * task runners: concepto, gulp y grunt. https://brunch.io/
  * Preparación de proyectos: yeoman
  * transpiler: babel
  * package bundlers: Webpack y Browserify, parcel
  * ofuscadores: UglifyJS
  * minificadores: minify
  * Concepto de aplicación isomorfica: meteor
  * El DOM: concepto. El BOM.
  * Progressive Web Apps de google
  * Generadores de código: Plataformas fullstack: JHipster
  * Mockups Tools: figma & Adobe XD
  * Javascript
    * Concepto de Javascript no obstrusivo
    * Arrays
    * Objetos
    * Funciones
    * Prototipos, herencia prototípica
    * Closures o cierres
    * Objeto global: objeto browser y objeto window
    * Objetos Wrappers: Math, Date, RegExpr, Json
    * Librerías importantes en Javascript: 
      * https://momentjs.com/
      * https://www.chartjs.org/
      * https://animejs.com/
      * https://popper.js.org/
      * https://leafletjs.com/
      * https://sweetalert.js.org/guides/
      * https://hammerjs.github.io/
      * https://animate.style/
      * https://revealjs.com/

## Entorno servidor 
  * Lenguajes: nodejs, Java, PHP, Phyton, Ruby, Perl, Go, Rust, Elixir, Erlang, Haskell, Clojure
  * Lenguajes para apps: Java, Dart, Flutter, React Native, Xamarin, Swift
  * Frameworks:
    * Java: Spring, Struts, Play, JSF, PrimeFaces, Tapestry, Vaadin, Openxava
    * Phyton: Django, Flask
    * Node: Express
    * Ruby: Rails
    * PHP: Laravel, CodeIgniter, Symphony, Cake, Yii, Zend, Phalcon, Slim
  * ORM: concepto y productos:
    * Java: Hibernate, EclipseLink, MyBatis
    * PHP: Doctrine
    * Node: Sequelize
  * Sistemas de gestión de dependencias: 
    * Java: Gradle, Maven, 
    * PHP: composer, PEAR...
    * Node: npm
  * Entorno Java
    * Java Virtual Machine
      * ¿Qué es la JVM?
      * Ventajas y desventajas de usar la JVM 
      * Lenguajes que compilan a bytecode: Java, Scala, Groovy, Kotlin
    * Concepto de Bytecode
    * JRE y JDK: concepto y diferencias
    * Gestores de dependencias: Gradle vs Maven
    * Spring vs Spring boot.
    * Spring security
    * Otros módulos de spring
    * Contenedores de servlets Java: Jetty, Tomcat, undertow...
    * Servidores de aplicaciones Java: JBoss, GlassFich, WebSphere, WildFly...
    * Concepto de servlet: 
      * objetos request y response. 
      * Métodos service e init.
      * El descriptor de despliegue web.xml
      * sesiones
    * Sistemas para gestionar logs en Java: Log4j, Log4j2, logBack

## Bases de datos 
  * Diferencia entre base de datos, SGBD y SGBDR
  * Sistemas gestores de bases de datos más importantes del mercado. 
    * Distinguir aquellos que son entornos libres.
    * Distinguir aquellos que son relacionales y los que no lo son.
  * APIs abiertas:
    * Firebase
    * GraphQL
  * SGBD NoSQL: 
    * Apache Cassandra
    * MongoDB
    * Redis
  * Concepto de campos autonuméricos. Claves. Claves ajenas.
  * Concepto de vista.
  * Diagramas de entidad-relación para modelar una base de datos relacional.
  * Formas normales, hasta la tercera forma normal.
  * Lenguajes DDL y DML.
  * Lenguaje de consulta SQL: inserciones, borrados, actualizaciones, consultas de una o varias tablas, alias, condiciones where, consultas agrupadas, consultas agrupadas y filtradas
  * Resultset
  * Transacciones
  * Prepared statements y la inyección de código.
  * GUI para mysql: Programas phpMyAdmin, MySQL Workbench, HeidiSQL, TOAD...








## Control de versiones 
  * Concepto. 
  * Ventajas que aportan los controladores de versiones
    * trazabilidad
    * historial de cambios
    * reversión
    * trabajo en grupo
    * trabajo en ramas
  * Herramientas
    * cvs
    * subversion svn
    * git
    * mercurial
  * Repositorios git
    * github
    * bitbucket
    * gitlab
==== Integración continua ====
  * Pruebas unitarias:
    * junit
    * phpunit
    * Mocha Jasmine Jest
  * Pruebas de integracion:
    * selenium
  * Servidores: Jenkins, Travis CI, TeamCity, CircleCI
  * Issue tracking: Jira, backlog, trac. Redmine, mantis
  * Teconologías para la inspección y la mejora del código: codeclimate, sonarqube,
==== Despliegue ====
  * Microservicios y Message Brokers: RabbitMQ, Kafka, Redis, SQS
  * Monitorización: new relic, datadog, dynatrace ...
  * Infraestructura:
    * iaas: Infraestructura como servicio: DigitalOcean, ovh, Linode, 
    * caas: Container as a service: AWS ECS, Azure, Google cloud
    * paas: Plataforma como servicio: Google App Engine, CloudFoundry, Heroku, AWS (Beanstalk), Azure
    * faas: funciones como servicio: AWS lambda, Azure functions, Google functions
    * saas: Software como servicio: gmail, salesforce, aplicaciones hospedadas (wordpress, magento, prestashop, joomla, drupal...)
  * Contenedores:
    * Docker y los contenedores
    * Docker compose
    * Docker swarm, Kubernetes



## Personajes
  * john resig
  * douglas crockford
  * Jeremy Ashkenas
  * misko hevery
  * Rod Johnson
  * James Goslin
  * Martin Fowler
  * Eric S. Raymond
  * Rasmus Lerdorf
  * john Papa

## Chronology

  * Chronology: https://github.com/vsmysee/awesome-it-history
