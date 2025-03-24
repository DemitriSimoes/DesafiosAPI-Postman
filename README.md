# DesafiosAPI-Postman
Criando testes de API no Postman, exportando arquivos .json das "collections" e dos "environments".

Os arquivos podem ser importados para o Postman ou podem rodar executando o Newman,
utilizando o comando:
newman run my-collection.json -e dev-environment.json


O arquivo "CTG.postman_collection.json" se relaciona com o ambiente "Local.postman_environment.json".

Comando Newman:
newman run CTG.postman_collection.json -e Local.postman_environment.json


O arquivo "JSONPlaceHolder.postman_collection.json" se relaciona com o ambiente "JSONPlaceHolder.postman_environment.json".

Comando Newman:
newman run JSONPlaceHolder.postman_collection.json -e JSONPlaceHolder.postman_environment.json
