# Swagger

Swagger tool is probably the most well-known of them all for documenting Rest APIs – its basically a REST API ecosystem consisting of several aspects:

The Swagger spec:
A way of documenting APIs using JSON
An Editor for designing API contracts first, i.e. before any code
A Web UI which takes a Swagger spec and dynamically converts it into API documentation in a web page
Many plugins for integrating Swagger with your language/framework of choice
Code generators for turning a Swagger spec into skeleton code (server and client)

Swagger with Java Library called Springfox which is designed to generate a Swagger spec from APIs built using the Spring framework. It does this by recognising the Spring REST annotations and converting these to the appropriate Swagger spec elements and then exposing an endpoint which, when called, returns the spec in json format. Springfox also supports the Swagger annotations (@Api, @ApiOperation etc) which enables you to provide additional details, e.g. descriptions.

It will reduce the overhead of updating the static pages (which we currently have) and will tally with the api changes on real time. 
1. Adding dependencies in pom file
2. Creating a SwaggerConfig class 
3. we need to define CORS filter(if Swagger UI is running from a different host domain)
4. Integrating it with Postman.
