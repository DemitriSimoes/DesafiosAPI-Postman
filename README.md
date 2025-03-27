# DesafiosAPI-Postman
Creating API tests in Postman, exporting .json files from "collections" and "environments".

Used two APIs, downloading and running one locally "api-clientes-example-microservico" from VinnyPessoni
and using another public "{JSON} Placeholder".

Files can be imported into Postman or run by running Newman,
using the command:

newman run my-collection.json -e dev-environment.json


The "CTG.postman_collection.json" file relates to the "Local.postman_environment.json" environment.
In this procedure, one of the GET methods (/risco/{id}) used "Basic Auth" authentication, with username and password.

Newman Command:

newman run CTG.postman_collection.json -e Local.postman_environment.json


The "JSONPlaceHolder.postman_collection.json" file relates to the "JSONPlaceHolder.postman_environment.json" environment.
In this procedure, the principle of limit value analysis was used in the first GET method (/post/{id}).
Returning for the lower limit -1 and for the upper limit +1 "404", as expected.

Newman Command:

newman run JSONPlaceHolder.postman_collection.json -e JSONPlaceHolder.postman_environment.json
